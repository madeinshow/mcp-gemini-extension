# Made In Show — Gemini CLI extension

Connect [Gemini CLI](https://geminicli.com) to your **Made In Show (MIS)** installation: ask about productions, warehouse availability, crew, company vehicles and finance data — and, if your administrator allows it, act on them — straight from your terminal. Every write asks you to confirm a preview first.

> **Italiano più sotto.** 🇮🇹

## Requirements

- A Made In Show account with AI access enabled by your administrator (access is off by default; the administrator decides per user whether the AI can view, view and act, or nothing).
- [Gemini CLI](https://geminicli.com) with a paid Gemini API key from [Google AI Studio](https://aistudio.google.com/apikey) (pay-as-you-go) or a Gemini Code Assist Standard/Enterprise license. Since 18 June 2026 free usage and Google AI Pro/Ultra subscriptions no longer give access to Gemini CLI.

## Install

```bash
gemini extensions install https://github.com/madeinshow/mcp-gemini-extension
```

On first use, authenticate with your Made In Show credentials:

```
/mcp auth mis
```

A browser window opens for the standard MIS login and consent. Tokens are stored locally by Gemini CLI and refreshed automatically.

## Privacy

The connector's privacy policy: <https://do.madeinshow.app/privacy>. Data you access through this extension flows through your own Gemini account under Google's terms — check your account's data settings.

## Support

<https://www.madeinshow.com>

---

## Italiano

Collega Gemini CLI alla tua installazione **Made In Show (MIS)**: produzioni, disponibilità di magazzino, crew e amministrazione — in una frase, dal terminale. L'accesso AI parte disabilitato: lo abilita il tuo amministratore, utente per utente (consultare, agire o nulla).

Requisiti: un account Made In Show con accesso AI abilitato e Gemini CLI con una API key Gemini a pagamento da [Google AI Studio](https://aistudio.google.com/apikey) (costo a consumo) oppure una licenza Gemini Code Assist Standard o Enterprise. Dal 18 giugno 2026 l'uso gratuito e gli abbonamenti Google AI Pro e Ultra non danno più accesso a Gemini CLI. Installazione e autenticazione come sopra. Privacy policy del connettore: <https://do.madeinshow.app/privacy>.
