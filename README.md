# Made In Show — Gemini CLI extension

Connect [Gemini CLI](https://geminicli.com) to your **Made In Show (MIS)** installation: ask about productions, warehouse availability, crew and finance data — and, if your administrator allows it, act on them — straight from your terminal.

> **Italiano più sotto.** 🇮🇹

## Requirements

- A Made In Show account with AI access enabled by your administrator (access is off by default; the administrator decides per user whether the AI can view, view and act, or nothing).
- [Gemini CLI](https://geminicli.com) with a free Gemini API key from [Google AI Studio](https://aistudio.google.com/apikey) (the CLI's individual Google sign-in has been deprecated by Google).

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

Requisiti: un account Made In Show con accesso AI abilitato e Gemini CLI con una API key Gemini gratuita da [Google AI Studio](https://aistudio.google.com/apikey) (il login Google individuale della CLI è stato deprecato da Google). Installazione e autenticazione come sopra. Privacy policy del connettore: <https://do.madeinshow.app/privacy>.
