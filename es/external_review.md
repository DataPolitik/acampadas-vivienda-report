# Revisión de canales externos: regla de etiquetado y resultado

<p class="lang" style="font-size:90%"><a href="../external_review.html">English</a> · <strong>Español</strong> · <a href="../ca/external_review.html">Català</a></p>

> Esta página trata del primer estudio, del 14 de septiembre al 5 de octubre de 2026. La movilización continuó: véase el [seguimiento](followup.md), del 6 de octubre a la huelga del 11 de noviembre.

Primer estudio, revisión hecha el 2026-10-05.
Evidencias y decisiones por canal: [evidencias por canal (CSV, en inglés)](../external_review_log.csv).

*Traducción del original en inglés.*

## Qué se revisó

Los 133 nodos que aparecieron en los grafos de reenvíos y enlaces fuera de la muestra
(«externos»): canales y grupos de los que los canales de la muestra reenviaron, a los que
mencionaron con @ o a los que enlazaron entre el 2026-09-14 y el 2026-10-05.

No se revisaron: las 5 cuentas de usuario vistas en grupos, los 3 orígenes de reenvíos
con nombre oculto y los 35 usuarios con @ que no se pudieron asociar a una cuenta de
Telegram.

## Evidencias

De cada canal externo se leyeron sus propias publicaciones desde el 2026-09-14 (sin los
mensajes reenviados, hasta 1.000 mensajes por canal; ninguno llegó al límite). Se hicieron
dos recuentos por palabras clave:

- `housing_posts`: vivienda, vivenda, habitatge, desahuci-, desnona-, acampad-,
  Maricarmen, inquilin-, llogat-, alquiler, lloguer, rentis-
- `camp_posts`: solo acampad- o Maricarmen

Se guarda como evidencia la primera publicación que coincide. Las coincidencias únicas se
leyeron para confirmar que trataban de las acampadas; se descartó un falso positivo (un
poema).

## Regla

1. **Prueba de implicación.** Un canal se añade a la muestra solo si tiene al menos una
   publicación propia sobre las acampadas o el desahucio de Maricarmen en la ventana. Que
   lo reenvíe un canal de la muestra no basta: un solo canal aliado (Red TEJAR) hace el
   44 % de todos los reenvíos.
2. **Etiqueta según el tipo de canal**, para los que pasan la prueba:
   - vivienda: organizaciones de vivienda (sindicatos de inquilinas, PAH, asambleas de
     vivienda).
   - aliado: organizaciones y colectivos que no son organizaciones de vivienda:
     partidos, sindicatos, centros sociales, agendas de movimientos, grupos de
     solidaridad y antirrepresivos.
   - aliado: canales personales de individuos, con la misma prueba que las
     organizaciones. No se consideran los usuarios que publican dentro de grupos.
   - medio: medios de información, revistas, editoriales y programas, incluidos los
     vinculados a partidos.
3. **Los agregadores y los chats se deciden leyendo sus mensajes**, no por su tipo:
   aliado si el canal habla como actor del movimiento (lanza o difunde llamamientos a la
   acción, publica comunicados de colectivos); no se añade si solo republica titulares o
   es conversación abierta entre participantes.
4. **No se añaden:** canales sin ninguna publicación sobre las acampadas, ruido y canales
   privados o sin nombre de usuario público (no se pueden leer).

## Resultado

| Decisión | Canales |
|---|---|
| Añadido como vivienda | 1 (PAH-VKS) |
| Añadido como aliado: organizaciones | 28 |
| Añadido como aliado: individuos | 8 |
| Añadido como aliado: agregador | 1 (Malditaultraderecha) |
| Añadido como medio | 23 |
| No añadido: sin publicaciones sobre las acampadas | 60 (42 organizaciones u otros, 12 medios, 5 individuos, 1 grupo) |
| No añadido: agregador / chat | 2 (chat de Malditaultraderecha, Revolución Comunista) |
| No añadido: no legible | 7 |
| No revisado: usuarios y nombres ocultos | 8 |

Cuatro canales que ya estaban en la muestra como aliados se reetiquetaron como medios
para aplicar la regla de forma uniforme: Kaosenlared, L'Accent, El Faradio, Multicanal
Radio.

Dos canales etiquetados como fuera de ámbito antes de que existiera la categoría de medio
se reetiquetaron después como medios: Nuestra España Noticias (un medio de información
general que cubrió las acampadas) y Geoestrategia y Política (un canal de comentario de
una sola persona; sus publicaciones sobre las acampadas son comentario de apoyo más que
llamamientos a la acción, así que medio y no aliado).

Muestra tras la revisión: 132 canales: 22 de vivienda, 79 aliados, 29 medios, 2 fuera de
ámbito (Roto2bot, un bot de hilos de un foro, y MEME_CCC, un canal de memes).

## Decisiones que requirieron juicio

- **Malditaultraderecha → aliado.** 67 publicaciones sobre las acampadas; publica
  llamamientos («Mañana ocupemos las plazas por todas las Maricarmen») y comunicados
  recibidos de colectivos.
- **Chat de Malditaultraderecha → no añadido.** 17 mensajes sobre las acampadas de 8
  participantes; conversación individual, en parte escéptica con la acampada.
- **Revolución Comunista → no añadido.** Sus 18 publicaciones sobre las acampadas son
  titulares y publicaciones de X republicados; no tiene voz propia.
- **Diario Socialista → medio.** Es el periódico del Movimiento Socialista, cuya
  organización juvenil (Coordinadora Juvenil Socialista) es un aliado con el canal vacío.
  Se etiqueta por tipo, pero es la principal voz de esa corriente en Telegram.
- **Agendas de movimientos → aliado.** Convocatorias Madrid, Convócala Málaga,
  Convocatorias Cádiz y Sevilla en Acción publican convocatorias más que noticias, así que
  se tratan como canales del movimiento, no como medios.
- **Editoriales y publicaciones periódicas de corrientes políticas → medio.**
  Traficantes de Sueños, Tierra y Libertad, Viento Sur, Poder Popular, Regeneración y
  similares.
- **Dos canales relevantes no se pudieron añadir:** Difusión Asamblea de Vivienda Sevilla
  (vivienda, 11 reenvíos) y el grupo Acampada Plaça Ajuntament (la acampada de València).
  Los dos son privados o no tienen nombre de usuario público.

## Límites

- Los recuentos por palabras clave no captan las publicaciones que son solo imágenes o
  que nombran la movilización de otra manera; un canal sin coincidencias puede haber
  participado igualmente.
- Una sola publicación sobre las acampadas basta para pasar la prueba; el registro da el
  recuento para que se pueda aplicar un umbral más estricto.
- No se añadieron canales por ninguna otra vía que esta revisión.

## Segunda ronda (2026-10-05)

Analizar los canales añadidos en la primera ronda trajo 85 canales nuevos al grafo. Los
85 se revisaron con las mismas evidencias y la misma regla; sus filas están marcadas como
ronda 2 en el registro.

| Decisión | Canales |
|---|---|
| Añadido como vivienda | 2 (Acampada per l'habitatge, el canal de la acampada de Barcelona; Sindicat Llogateres Mallorca) |
| Añadido como aliado: organizaciones | 9 |
| Añadido como aliado: agregadores | 3 |
| Añadido como medio | 21 |
| No añadido: sin publicaciones sobre las acampadas | 46 (38 organizaciones u otros, 8 medios) |
| No añadido: agregadores | 2 |
| No añadido: no legible | 2 |

Muestra tras la segunda ronda: 167 canales: 24 de vivienda, 91 aliados, 50 medios, 2
fuera de ámbito.

Decisiones que requirieron juicio:

- **Canales de comentario e información → medio**, siguiendo la decisión sobre
  Geoestrategia y Política: España en Guerra, Fullblack161, Prima Linea,
  GlobalRevolution, Anarquismo & Antimilitarismo.
- **Agregadores que difunden llamamientos → aliado:** Antifascistas, Mitxis na Galiza
  Antifascista, Presos Revolucionarios. **Agregadores que solo republican → no
  añadidos:** Notice (Todos con Rusia), FemiNews.
- **Grupo Ruptura → aliado, con una salvedad.** Pasa la prueba de implicación, pero su
  publicación es crítica con la acampada. La regla mide la implicación, no la postura.
- **elPlural.com → medio**, aunque el canal es un espejo no oficial de la web.
- **Falsos positivos descartados:** Red Antiespecista Madrid (una acampada animalista en
  el Reino Unido) y L'Àgora Es Queda Al Barri (una acampada contra su propio desalojo, el
  14 y el 15 de octubre).

La red recoge ahora la categoría y la decisión de revisión de cada canal revisado, así
que los canales revisados y no añadidos siguen etiquetados.

La revisión no se ha repetido con los nodos que aportó el análisis de los canales
añadidos en la segunda ronda.

**Cómo citar esta página.**

<div class="citation" style="font-size:90%;border-left:3px solid #d0d7de;padding:6px 12px;margin:0 0 16px"><p class="cite-text" style="margin:0">DataPolitik (Heurística). <em>Revisión de canales externos: regla de etiquetado y resultado</em>. En <em>Acampadas por la vivienda y redes de comunicación en Telegram en España, otoño de 2026</em>. Periodo de observación: 14 de septiembre – 5 de octubre de 2026. Publicado el 7 de noviembre de 2026. <a href="https://datapolitik.github.io/acampadas-vivienda-report/es/external_review.html">https://datapolitik.github.io/acampadas-vivienda-report/es/external_review.html</a></p></div>

Texto y figuras originales: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) · [Uso y citación](index.md#use-and-citation)

---

<div style="display:flex;align-items:center;gap:20px;flex-wrap:wrap;margin:8px 0 10px"><a href="https://www.heuristica.barcelona/datapolitik/"><img src="../figures/brand/datapolitik.png" alt="DataPolitik" height="32" style="display:block"></a><a href="https://www.heuristica.barcelona/"><img src="../figures/brand/heuristica.png" alt="Heurística" height="16" style="display:block"></a></div>

Un estudio de [DataPolitik](https://www.heuristica.barcelona/datapolitik/), de [Heurística](https://www.heuristica.barcelona/). · [Inicio](index.md) · [Presentación del seguimiento](followup.md)
