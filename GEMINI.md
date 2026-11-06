# Made In Show (MIS) — context for Gemini

This extension connects you to a Made In Show (MIS) installation via the official MIS MCP connector.

- MIS is an Italian management platform for live-event production companies (service audio/video/luci): productions, quotes and final statements, warehouse, crew, vehicles, invoicing. Backend messages are in Italian.
- Start with `mis_status` to see the connected installation, the user identity and what the user's AI access allows. If more than one installation is available, tools accept an `installation` parameter.
- Access is governed server-side by MIS (`ai_level`, per user): the AI may be allowed to view only, to view and act, or nothing. A 403 from the connector means the MIS administrator has not granted that capability — do not retry, tell the user to ask their administrator.
- Prefer the curated `mis_*` tools over generic requests. Read tools cover productions and their whole picture (`mis_get_production_overview`: working days, tags, crew, vehicles, consumables, linked invoices, each section with its own status), warehouse and availability, crew and company vehicles, courses, calendar, invoices and statistics.
- Every write is a two-step confirmation: the first call returns a preview and a `confirmation_token` and writes nothing; repeat the same arguments with `confirm=true` and that token to apply it. Bookings re-read the data afterwards and report an uncertain outcome when the result does not match the preview.
- Never pick the first match: when a customer, technician, vehicle or rate is ambiguous the tool returns candidates and no token. Show them and ask the user which one.
- Booking a vehicle or a technician replaces that resource's whole presence on the production, so the preview lists every day being removed, including days outside the working window. Read it to the user before confirming. Conflicts with confirmed bookings or unavailability block the write unless the user explicitly accepts them.
- Amounts and rates appear only for users with the economic-data permission, and their absence is stated. No tool sends notifications or emails.
- Answer with data returned by the tools; do not guess values MIS can provide.
