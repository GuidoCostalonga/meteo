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

## Comuni

Tutti i 215 Comuni della regione, raggruppati per provincia nel menu a tendina:
Gorizia 25, Pordenone 50, Trieste 6, Udine 134. Roveredo in Piano, Pordenone e
Trieste restano raggiungibili con un tocco. La pagina ricorda l'ultimo comune scelto
sul dispositivo di chi la consulta.

## Fonti

- **Previsioni:** [Open-Meteo](https://open-meteo.com/), che distribuisce le corse dei
  modelli ECMWF IFS, ICON-D2 del Deutscher Wetterdienst e Météo-France. Fuso orario
  Europe/Rome, aggiornamento automatico ogni quindici minuti.
- **Elenco dei Comuni:** codici ISTAT delle unità amministrative territoriali.
- **Coordinate:** centroide del municipio di ciascun Comune, standard EPSG:4326,
  dalla raccolta [comuni-italiani](https://github.com/opendatasicilia/comuni-italiani)
  di Open Data Sicilia.

L'elenco è stato verificato incrociando due archivi indipendenti: 215 Comuni, stessi
codici ISTAT e stesse denominazioni in entrambi.

## Tecnica

Pagina singola, senza dipendenze esterne: HTML, CSS e JavaScript in un unico file.
I dati arrivano dall'interfaccia pubblica di Open-Meteo, senza chiave di accesso.

## Avvertenza

Le previsioni indicano probabilità, non certezze. Per le allerte ufficiali di
protezione civile fare sempre riferimento alla Protezione Civile della Regione
Friuli Venezia Giulia.
