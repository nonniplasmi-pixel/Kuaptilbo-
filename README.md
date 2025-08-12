# Kauptilboð Demo (Vercel)

Þetta er einföld prufusíða sem leyfir þér að hlaða upp PDF kauptilboði og lesa texta (PDF textalag eða OCR).

## Hýsa á Vercel (ókeypis)
1. Farðu á https://vercel.com og skráðu þig inn.
2. Smelltu **New Project** → **Import** → **Add New…** → **Deploy from Git** eða **Deploy** frá ZIP.
   - Auðveldast: **Create a new project** → dragðu ZIP sem fylgir þessari skrá inn í Vercel.
3. Vercel finnur `index.html` og notar `@vercel/static`. Smelltu **Deploy**.
4. Þú færð slóð, t.d. `https://kauptilbod-demo.vercel.app`.

## Keyra local (valfrjálst)
1. Opnaðu flugstöð í möppunni.
2. Python 3: `python -m http.server 8000`
3. Opnaðu `http://localhost:8000` í vafra.

## Notkun
- Opnaðu síðuna → Hladdu upp PDF → Kerfið reynir að ná texta.
- Ef PDF er skannað (mynd), virkjast OCR sjálfkrafa.
- Breyttu reitum handvirkt ef þarf. JSON hægra megin uppfærir sig sjálfkrafa.

## Athugið
- Engin gögn eru send á netþjón; allt keyrir í vafranum og sækir bókasöfn frá CDN.
