# Sito Black Panther — cosa è cambiato

Aggiornato il **07/10/2026**, partendo dalla versione pubblicata su GitHub
(commit `38f236a`).

## File modificati

Soltanto due, e sono lo stesso file:

- `flyer.html`
- `flayer.html` (copia identica, con il nome scritto male)

Tutto il resto del sito è **intatto**, com'era su GitHub.

## Cosa è stato corretto

La pagina delle locandine leggeva i nomi dei file pretendendo questa forma:

```
2026-03-16_EDM_TECHNO_NomeEvento.png
```

cioè **tre parti** separate da underscore. I file veri nella cartella `flyers/`
sono però scritti in **due parti**, con uno spazio dentro:

```
2026-03-16_EDM TECHNO.png
```

Nessuno dei quindici file passava il controllo: finivano tutti insieme in un
gruppo chiamato "VARIO", senza data e in fondo alla pagina.

Adesso la pagina accetta **entrambe le forme** — quella scritta a mano e quella
che produce il bot — e le otto locandine vere compaiono con data e genere:

```
2026-03-16   EDM TECHNO
2026-03-23   ROCK
2026-03-30   80 90 DISCO
2026-04-06   EDM TECHNO
2026-04-13   ROCK
2026-04-20   80 90 DISCO
2026-04-27   EDM TECHNO
2026-05-04   ROCK
```

I sette file chiamati `Screenshot 2026-…` non hanno un formato riconoscibile e
finiscono sotto "ALTRO". Se sono locandine vere, basta rinominarli così:

```
2026-05-09_ROCK.png
```

e si sistemano da soli.

## Attenzione prima di pubblicare

Questo zip parte dalla versione **su GitHub**. Se sul tuo computer hai modifiche
più recenti che non hai ancora caricato, non sovrascrivere tutto: copia solo
`flyer.html` e `flayer.html`.
