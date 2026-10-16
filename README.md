# El fil de la llum

Aventura gràfica original en català, inspirada en la vida de **Josefa Tolrà i Abril**. Amb viatges entre el Maresme de 1956 i el Cabrils de 2026, amb catorze escenaris entre Cabrils, Vilassar de Dalt i Vilassar de Mar.

**Jugar:** https://skirep.github.io/el-fil-de-la-llum/

## L’aventura

La Clara, una jove enquadernadora fictícia de 2026, travessa una espiral temporal i ajuda la Pepeta a recuperar tres fulls d’un quadern dispers pel vent. Per relligar-lo necessita tant els fulls del passat com la memòria compartida del present. Tres actes, vuit personatges amb diàlegs ramificats, inventari combinable, enigmes sense morts ni bloquejos irreversibles, un duel d’insults amb espases de paper i rèpliques enginyoses originals, pistes graduals, quadern de notes, mapa, desament automàtic i música ambiental original sintetitzada.

Durada objectiu: aproximadament 30 minuts en una primera partida, segons lectura, exploració i pistes. No s’ha validat amb una prova de durada amb jugadors externs.

### Llocs

- Cabrils: Santa Creu, carrer de Sant Salvador, Ca l’Arlot, safareig del torrent Roig, ermita de Sant Cristòfol i mirador del Montcabrer.
- Cabrils actual: restaurant La Concòrdia, Casal de la Gent Gran, Centre Cívic La Fàbrica, plaça del Mil·lenari de Catalunya, Escola Mas Maria i Escola L’Olivera. Tots tenen interaccions obligatòries en la cadena temporal. Les Escoles Tolrà apareixen en un record del passat.
- Vilassar de Mar: platja i Torre d’en Nadal.
- Vilassar de Dalt: taller tèxtil i casa d’un enquadernador, interiors ficticis que evoquen el patrimoni local.

Els escenaris són interpretacions artístiques, no reconstruccions arquitectòniques o geogràfiques exactes. No són fotografies ni reproduccions d’obres de Tolrà. Pixel art generat per a aquest joc i personatges animats dibuixats per codi. L’evocació de les aventures clàssiques no utilitza personatges, codi, música ni assets de LucasArts.

## Controls

Clicar o tocar per explorar. Accions Mirar, Parlar, Agafar i Usar. Seleccionar un objecte de l’inventari i després el destí; per combinar, seleccionar dos objectes. `M`: mapa de l’època actual. Botó `Època`: viatjar entre 2026 i 1956 després de tocar l’espiral. `Q`: quadern. `Esc`: cancel·lar/tancar. `Tab` i `Enter`: navegar i activar punts interactius. «Mostrar objectes» revela les zones interactives. So opcional; sense gravacions ni connexió a serveis de joc.

El desament usa localStorage del navegador. No hi ha comptes ni servidor. El codi no envia telemetria. Les tipografies opcionals de Google Fonts poden substituir-se per les fonts locals de reserva.

## Història i ficció

Josefa Tolrà (Cabrils, 1880–1959) va ser treballadora tèxtil i una creadora autodidacta vinculada al dibuix, l’escriptura, el brodat i l’espiritualitat. Els anys finals a Ca l’Arlot i la vinculació amb Cabrils tenen base documental. Els viatges temporals són una fantasia narrativa sense atribució de poders reals a Josefa. El quadern, els viatges, els enigmes, la Clara i tots els diàlegs són ficció. La Nora i la Joana no representen treballadors ni usuaris reals. Les mostres escolars i el taller del centre cívic també són inventats. Les veus mediúmniques es presenten com la vivència personal de l’artista, no com un fet sobrenatural provat.

Fonts consultades el 16 d’octubre de 2026:

- [Itinerari urbà Josefa Tolrà, Ajuntament de Cabrils](https://www.cabrils.cat/itinerari-josefa-tolra/cat)
- [Josefa Tolrà, MACBA](https://www.macba.cat/es/actor/josefa-tolra/)
- [Cabrils i la seva història](https://www.cabrils.cat/municipi/informacio-del-municipi/cabrils-i-la-seva-historia)
- [Sant Cristòfol, Diputació de Barcelona](https://patrimonicultural.diba.cat/element/capella-de-sant-cristofol)
- [Torre d’en Nadal, Ajuntament de Vilassar de Mar](https://www.vilassardemar.cat/actualitat/noticies/tres-plafons-al-carrer-recorden-les-tres-torres-de-defensa-que-hi-havia)

## Desenvolupament

HTML, CSS i JavaScript modular sense dependències de runtime. Servir l’arrel amb qualsevol servidor estàtic (els mòduls no funcionen obrint directament un fitxer `file://`).

```sh
python3 -m http.server 8080
npm test
```

GitHub Pages: branca `main`, directori `/ (root)`, amb `.nojekyll`. Els tests validen la cadena completa, la persistència, les dependències, les combinacions i rutes alternatives. Vegeu `WALKTHROUGH.md` per a la solució.

## Crèdits d’art

Fons originals creats amb la generació d’imatges integrada. `assets/maresme.webp`: atlas de plaça, estudi, safareig, taller, platja i enquadernador. `assets/cabrils.webp`: Sant Cristòfol i Montcabrer. Especificació: escena històrica mediterrània de 1956, pixel art d’aventura 2D amb llums ambre i ombres turquesa; sense persones, textos ni reproduccions d’obres existents. Sprites i música: originals per codi.

## Fonts dels espais actuals

- [La Concòrdia, Associació d’Hostalers de Cabrils](https://hostalersdecabrils.com/restaurant-la-concordia/)
- [La Concòrdia, memòria digital municipal](https://memoriadigital.cabrils.cat/tag/la-concordia/)
- [Casal i La Fàbrica, agenda municipal](https://www.cabrils.cat/actualitat/agenda)
- [Escola Mas Maria, web del centre](https://agora.xtec.cat/escolamasmaria/lescola/)
- [Escola L’Olivera, web del centre](https://agora.xtec.cat/escolaolivera/)
- [Plaça del Mil·lenari, cartografia municipal](https://www.cabrils.cat/media/repository/POUM/Normes_urbanistiques._Annex_I.pdf)

`assets/present.webp`: sis escenaris originals del Cabrils actual, creats amb la generació d’imatges integrada. Prompt: atlas de sis espais comunitaris actuals en pixel art mediterrani amb llum daurada i ombres turquesa, sense persones ni logos; interpretacions artístiques de La Concòrdia, el casal, La Fàbrica, la plaça i les dues escoles.

## Duel d’insults

El Capità Desmemòria és un antagonista fantàstic original que guarda el full del cel al Montcabrer de 1956. El duel té animació de dues figures amb espases de paper, atacs, parades, espurnes i un efecte sonor si el so està activat. Cada provocació proposa tres rèpliques: la correcta gira la metàfora del rival. Primera persona amb tres punts guanya. Una derrota permet repetir sense perdre objectes. Sis provocacions i divuit rèpliques originals; cap text de Monkey Island ni altres jocs s’ha reutilitzat.
