# Cantina Insights

Crea una Dashboard PWA mobile-first per il progetto "Cantina Cerzasauro". Usa React, Tailwind CSS, shadcn/ui e lucide-react per le icone. Il design deve avere un tema scuro elegante e premium (sfondo slate-950, pannelli glassmorphism in slate-900) con accenti color rosso vino/bordeaux (rose-600) per richiamare il settore vitivinicolo.

L'app deve connettersi in tempo reale a Supabase usando @supabase/supabase-js.
URL: [https://meidwoskxfvwnpomrrre.supabase.co](https://meidwoskxfvwnpomrrre.supabase.co)
KEY: sb_publishable_U7or0vjLYPPTgCgcgqZnCw_MMSOf3bb

La UI deve avere una singola colonna scorrevole con queste 3 sezioni principali:

Header e Statistiche Live (Lettura tabella statistiche):
Connettiti alla tabella statistiche (dove id=1). Mostra un grande indicatore circolare o una barra di progresso per le "Email Inviate Oggi" rispetto all'"Obiettivo Oggi" (es. 24/50). Affianco, mostra un piccolo badge con i "Crediti Tavily" residui.

Risposte in Arrivo (Lettura tabella risposte):
Crea una sezione per i messaggi in arrivo dai ristoratori. Leggi i dati dalla tabella risposte ordinandoli per data_ricezione decrescente. Mostra una lista elegante a card con il mittente, l'oggetto e l'anteprima del messaggio.

Radar Ristoranti (Lettura tabella storico_email):
Crea una sezione per lo storico degli invii. Leggi i dati dalla tabella storico_email ordinandoli per data_invio decrescente (limit=15). Per ogni riga, mostra l'icona di una spunta di successo, il nome_locale in grassetto e la email_locale in piccolo.

Implementa il realtime di Supabase in modo che se l'agente Python in background aggiorna il database, i numeri e le liste sulla dashboard si aggiornino da soli senza dover ricaricare la pagina. Aggiungi stati di loading eleganti (skeleton) mentre i dati vengono scaricati da Supabase.

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/e8af29be-566e-408f-9328-33b92b40679c).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
