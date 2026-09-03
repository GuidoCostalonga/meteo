# Meteo FVG

Previsioni meteo per tutti i 215 Comuni del Friuli Venezia Giulia, con il confronto
fra i principali modelli europei.

**Online:** https://costalonga.org/meteo/

## Che cosa contiene

- **Adesso** — temperatura, temperatura percepita, vento e umidità del comune scelto
- **Attendibilità a 24 ore** — indice da 45 a 96 calcolato sulla dispersione fra i
  modelli ICON-D2 (DWD), ECMWF IFS e Météo-France: più i modelli concordano, più
  alto è il punteggio
- **Prossime ore** — 18 ore con temperatura, percepita e probabilità di pioggia
- **Prossimi 7 giorni** — minime, massime e probabilità di pioggia, con il dettaglio
  orario di ogni giorno selezionabile
- **Da sapere** — tre indicazioni pratiche su pioggia, vento e temperatura
- **Allerta della Protezione Civile** — il riquadro ufficiale pubblicato dalla
  Protezione Civile della Regione Friuli Venezia Giulia, riferito al comune scelto

## Comuni

Tutti i 215 Comuni della regione, raggruppati per provincia nel menu a tendina:
Gorizia 25, Pordenone 50, Trieste 6, Udine 134. Roveredo in Piano, Pordenone e
Trieste restano raggiungibili con un tocco. La pagina ricorda l'ultimo comune scelto
sul dispositivo di chi la consulta.

## Collegamento diretto per Comune

Ogni comune ha un proprio indirizzo, formato dal nome in minuscolo con i trattini
al posto degli spazi:

```
https://costalonga.org/meteo/#tarvisio
https://costalonga.org/meteo/#roveredo-in-piano
https://costalonga.org/meteo/#san-vito-al-tagliamento
```

Chi apre il collegamento trova la pagina già sul comune indicato. Il tasto **Copia
il collegamento** mette negli appunti l'indirizzo del comune visualizzato, pronto da
mandare per messaggio. L'indirizzo si aggiorna da solo a ogni cambio di comune.

I 215 identificativi sono tutti distinti: nessuna sovrapposizione fra comuni.

## Fonti

- **Previsioni:** [Open-Meteo](https://open-meteo.com/), che distribuisce le corse dei
  modelli ECMWF IFS, ICON-D2 del Deutscher Wetterdienst e Météo-France. Fuso orario
  Europe/Rome, aggiornamento automatico ogni quindici minuti.
- **Elenco dei Comuni:** codici ISTAT delle unità amministrative territoriali.
- **Coordinate:** centroide del municipio di ciascun Comune, standard EPSG:4326,
  dalla raccolta [comuni-italiani](https://github.com/opendatasicilia/comuni-italiani)
  di Open Data Sicilia.
- **Allerte:** riquadro ufficiale della Protezione Civile della Regione Friuli
  Venezia Giulia ([protezionecivile.fvg.it](https://www.protezionecivile.fvg.it/)),
  richiamato con il codice ISTAT del comune privato dello zero iniziale.

L'elenco è stato verificato incrociando due archivi indipendenti: 215 Comuni, stessi
codici ISTAT e stesse denominazioni in entrambi.

## Tecnica

Pagina singola, senza dipendenze esterne: HTML, CSS e JavaScript in un unico file.
I dati arrivano dall'interfaccia pubblica di Open-Meteo, senza chiave di accesso.

## Avvertenza

Le previsioni indicano probabilità, non certezze. Per le allerte ufficiali di
protezione civile fare sempre riferimento alla Protezione Civile della Regione
Friuli Venezia Giulia.
