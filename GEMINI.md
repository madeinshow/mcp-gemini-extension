# Made in Show (MIS) — context for Gemini

This extension connects you to a Made in Show (MIS) installation via the official MIS MCP connector.

- MIS is an Italian management platform for live-event production companies (service audio/video/luci): productions, quotes and final statements, warehouse, crew, vehicles, invoicing. Backend messages are in Italian.
- Start with `mis_status` to see the connected installation, the user identity and what the user's AI access allows. If more than one installation is available, tools accept an `installation` parameter.
- Access is governed server-side by MIS (`ai_level`, per user): the AI may be allowed to view only, to view and act, or nothing. A 403 from the connector means the MIS administrator has not granted that capability — do not retry, tell the user to ask their administrator.
- Prefer the curated `mis_*` tools over generic requests. Write operations are explicit: `mis_create_production` requires a two-step confirmation (`confirm=false` first returns a summary and writes nothing).
- Answer with data returned by the tools; do not guess values MIS can provide.
