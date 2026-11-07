# Revisió de canals externs: regla d'etiquetatge i resultat

<p class="lang" style="font-size:90%"><a href="../external_review.html">English</a> · <a href="../es/external_review.html">Español</a> · <strong>Català</strong></p>

> Aquesta pàgina tracta del primer estudi, del 14 de setembre al 5 d'octubre del 2026. La mobilització va continuar: vegeu el [seguiment](followup.md), del 6 d'octubre a la vaga de l'11 de novembre.

Primer estudi, revisió feta el 2026-10-05.
Evidències i decisions per canal: [evidències per canal (CSV, en anglès)](../external_review_log.csv).

*Traducció de l'original en anglès.*

## Què es va revisar

Els 133 nodes que van aparèixer als grafs de reenviaments i enllaços fora de la mostra
(«externs»): canals i grups dels quals els canals de la mostra van reenviar, que van
mencionar amb @ o als quals van enllaçar entre el 2026-09-14 i el 2026-10-05.

No es van revisar: els 5 comptes d'usuari vistos en grups, els 3 orígens de reenviaments
amb nom ocult i els 35 usuaris amb @ que no es van poder associar a cap compte de
Telegram.

## Evidències

De cada canal extern es van llegir les seves pròpies publicacions des del 2026-09-14
(sense els missatges reenviats, fins a 1.000 missatges per canal; cap no va arribar al
límit). Es van fer dos recomptes per paraules clau:

- `housing_posts`: vivienda, vivenda, habitatge, desahuci-, desnona-, acampad-,
  Maricarmen, inquilin-, llogat-, alquiler, lloguer, rentis-
- `camp_posts`: només acampad- o Maricarmen

Es desa com a evidència la primera publicació que coincideix. Les coincidències úniques
es van llegir per confirmar que tractaven de les acampades; es va descartar un fals
positiu (un poema).

## Regla

1. **Prova d'implicació.** Un canal s'afegeix a la mostra només si té almenys una
   publicació pròpia sobre les acampades o el desnonament de Maricarmen a la finestra. Que
   el reenviï un canal de la mostra no n'hi ha prou: un sol canal aliat (Red TEJAR) fa el
   44 % de tots els reenviaments.
2. **Etiqueta segons el tipus de canal**, per als que passen la prova:
   - habitatge: organitzacions d'habitatge (sindicats de llogateres, PAH, assemblees
     d'habitatge).
   - aliat: organitzacions i col·lectius que no són organitzacions d'habitatge: partits,
     sindicats, centres socials, agendes de moviments, grups de solidaritat i
     antirepressius.
   - aliat: canals personals d'individus, amb la mateixa prova que les organitzacions. No
     es consideren els usuaris que publiquen dins de grups.
   - mitjà: mitjans d'informació, revistes, editorials i programes, inclosos els
     vinculats a partits.
3. **Els agregadors i els xats es decideixen llegint-ne els missatges**, no pel tipus:
   aliat si el canal parla com a actor del moviment (llança o difon crides a l'acció,
   publica comunicats de col·lectius); no s'afegeix si només republica titulars o és
   conversa oberta entre participants.
4. **No s'afegeixen:** canals sense cap publicació sobre les acampades, soroll i canals
   privats o sense nom d'usuari públic (no es poden llegir).

## Resultat

| Decisió | Canals |
|---|---|
| Afegit com a habitatge | 1 (PAH-VKS) |
| Afegit com a aliat: organitzacions | 28 |
| Afegit com a aliat: individus | 8 |
| Afegit com a aliat: agregador | 1 (Malditaultraderecha) |
| Afegit com a mitjà | 23 |
| No afegit: sense publicacions sobre les acampades | 60 (42 organitzacions o altres, 12 mitjans, 5 individus, 1 grup) |
| No afegit: agregador / xat | 2 (xat de Malditaultraderecha, Revolución Comunista) |
| No afegit: no llegible | 7 |
| No revisat: usuaris i noms ocults | 8 |

Quatre canals que ja eren a la mostra com a aliats es van reetiquetar com a mitjans per
aplicar la regla de manera uniforme: Kaosenlared, L'Accent, El Faradio, Multicanal Radio.

Dos canals etiquetats com a fora d'àmbit abans que existís la categoria de mitjà es van
reetiquetar després com a mitjans: Nuestra España Noticias (un mitjà d'informació general
que va cobrir les acampades) i Geoestrategia y Política (un canal de comentari d'una sola
persona; les seves publicacions sobre les acampades són comentari de suport més que crides
a l'acció, per tant mitjà i no aliat).

Mostra després de la revisió: 132 canals: 22 d'habitatge, 79 aliats, 29 mitjans, 2 fora
d'àmbit (Roto2bot, un bot de fils d'un fòrum, i MEME_CCC, un canal de mems).

## Decisions que van requerir judici

- **Malditaultraderecha → aliat.** 67 publicacions sobre les acampades; publica crides
  («Mañana ocupemos las plazas por todas las Maricarmen») i comunicats rebuts de
  col·lectius.
- **Xat de Malditaultraderecha → no afegit.** 17 missatges sobre les acampades de 8
  participants; conversa individual, en part escèptica amb l'acampada.
- **Revolución Comunista → no afegit.** Les seves 18 publicacions sobre les acampades són
  titulars i publicacions d'X republicats; no té veu pròpia.
- **Diario Socialista → mitjà.** És el diari del Movimiento Socialista, l'organització
  juvenil del qual (Coordinadora Juvenil Socialista) és un aliat amb el canal buit.
  S'etiqueta per tipus, però és la principal veu d'aquell corrent a Telegram.
- **Agendes de moviments → aliat.** Convocatorias Madrid, Convócala Málaga,
  Convocatorias Cádiz i Sevilla en Acción publiquen convocatòries més que notícies, de
  manera que es tracten com a canals del moviment, no com a mitjans.
- **Editorials i publicacions periòdiques de corrents polítics → mitjà.** Traficantes de
  Sueños, Tierra y Libertad, Viento Sur, Poder Popular, Regeneración i similars.
- **Dos canals rellevants no es van poder afegir:** Difusión Asamblea de Vivienda Sevilla
  (habitatge, 11 reenviaments) i el grup Acampada Plaça Ajuntament (l'acampada de
  València). Tots dos són privats o no tenen nom d'usuari públic.

## Límits

- Els recomptes per paraules clau no capten les publicacions que són només imatges o que
  anomenen la mobilització d'una altra manera; un canal sense coincidències pot haver-hi
  participat igualment.
- Una sola publicació sobre les acampades n'hi ha prou per passar la prova; el registre
  dona el recompte perquè s'hi pugui aplicar un llindar més estricte.
- No es van afegir canals per cap altra via que aquesta revisió.

## Segona ronda (2026-10-05)

Analitzar els canals afegits a la primera ronda va portar 85 canals nous al graf. Tots
85 es van revisar amb les mateixes evidències i la mateixa regla; les seves files estan
marcades com a ronda 2 al registre.

| Decisió | Canals |
|---|---|
| Afegit com a habitatge | 2 (Acampada per l'habitatge, el canal de l'acampada de Barcelona; Sindicat Llogateres Mallorca) |
| Afegit com a aliat: organitzacions | 9 |
| Afegit com a aliat: agregadors | 3 |
| Afegit com a mitjà | 21 |
| No afegit: sense publicacions sobre les acampades | 46 (38 organitzacions o altres, 8 mitjans) |
| No afegit: agregadors | 2 |
| No afegit: no llegible | 2 |

Mostra després de la segona ronda: 167 canals: 24 d'habitatge, 91 aliats, 50 mitjans, 2
fora d'àmbit.

Decisions que van requerir judici:

- **Canals de comentari i informació → mitjà**, seguint la decisió sobre Geoestrategia y
  Política: España en Guerra, Fullblack161, Prima Linea, GlobalRevolution, Anarquismo &
  Antimilitarismo.
- **Agregadors que difonen crides → aliat:** Antifascistas, Mitxis na Galiza
  Antifascista, Presos Revolucionarios. **Agregadors que només republiquen → no
  afegits:** Notice (Todos con Rusia), FemiNews.
- **Grupo Ruptura → aliat, amb una reserva.** Passa la prova d'implicació, però la seva
  publicació és crítica amb l'acampada. La regla mesura la implicació, no la postura.
- **elPlural.com → mitjà**, tot i que el canal és un mirall no oficial del web.
- **Falsos positius descartats:** Red Antiespecista Madrid (una acampada animalista al
  Regne Unit) i L'Àgora Es Queda Al Barri (una acampada contra el seu propi
  desallotjament, el 14 i el 15 d'octubre).

La xarxa recull ara la categoria i la decisió de revisió de cada canal revisat, de manera
que els canals revisats i no afegits continuen etiquetats.

La revisió no s'ha repetit amb els nodes que va aportar l'anàlisi dels canals afegits a
la segona ronda.

---

<div style="display:flex;align-items:center;gap:20px;flex-wrap:wrap;margin:8px 0 10px"><a href="https://www.heuristica.barcelona/datapolitik/"><img src="../figures/brand/datapolitik.png" alt="DataPolitik" height="32" style="display:block"></a><a href="https://www.heuristica.barcelona/"><img src="../figures/brand/heuristica.png" alt="Heurística" height="16" style="display:block"></a></div>

Un estudi de [DataPolitik](https://www.heuristica.barcelona/datapolitik/), d'[Heurística](https://www.heuristica.barcelona/). · [Inici](index.md) · [Presentació del seguiment](followup.md)
