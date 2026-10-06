# External channel review — tagging rule and outcome

Project `acampadas_vivienda`, review run on 2026-10-05.
Per-channel evidence and decisions: [external_review_log.csv](external_review_log.csv).

## What was reviewed

The 133 nodes that appeared in the forward and link graphs without being project
channels ("external"): channels and groups that project channels forwarded from,
@-mentioned or linked to between 2026-09-14 and 2026-10-05.

Not reviewed: the 5 user accounts seen in groups, the 3 hidden-name forward origins,
and the 35 @-handles that could not be matched to a Telegram account.

## Evidence

For each external channel, its own posts since 2026-09-14 were read (forwarded
messages excluded, up to 1,000 messages per channel; none reached the cap). Two counts
were taken by keyword:

- `housing_posts`: vivienda, vivenda, habitatge, desahuci-, desnona-, acampad-,
  Maricarmen, inquilin-, llogat-, alquiler, lloguer, rentis-
- `camp_posts`: acampad- or Maricarmen only

The first matching post is kept as evidence. Single hits were read to confirm they
are about the camps; one false positive (a poem) was discarded.

## Rule

1. **Engagement test.** A channel is added to the project only if it has at least one
   own post about the camps or the Maricarmen eviction in the window. Being forwarded
   by a project channel is not enough: one ally channel alone (Red TEJAR) accounts for
   44% of all forwards.
2. **Tag by kind of channel**, for those that pass the test:
   - `in-scope` — housing organisations (tenant unions, PAH, housing assemblies).
   - `ally` — organisations and collectives that are not housing organisations:
     parties, unions, social centres, movement agendas, solidarity and anti-repression
     groups.
   - `ally` — personal channels of individuals, under the same test as organisations.
     Users posting inside groups are not considered.
   - `media` — news outlets, magazines, publishers and programmes, including
     party-linked ones.
3. **Aggregators and chats are decided by reading their messages**, not by kind:
   `ally` if the channel speaks as a movement actor (issues or relays calls to action,
   publishes collectives' statements); not added if it only reposts headlines or is
   open chatter among participants.
4. **Not added:** channels with no camp post, noise, and channels that are private or
   have no public username (tgmon cannot scan them).

## Outcome

| Decision | Channels |
|---|---|
| Added as `in-scope` | 1 (PAH-VKS) |
| Added as `ally` — organisations | 28 |
| Added as `ally` — individuals | 8 |
| Added as `ally` — aggregator | 1 (Malditaultraderecha) |
| Added as `media` | 23 |
| Not added — no camp post | 60 (42 organisations or other, 12 media, 5 individuals, 1 group) |
| Not added — aggregator / chat | 2 (Malditaultraderecha chat, Revolución Comunista) |
| Not added — unreadable | 7 |
| Not reviewed — users and hidden names | 8 |

Four channels already in the project as `ally` were retagged `media` so the rule is
applied uniformly: Kaosenlared, L'Accent, El Faradio, Multicanal Radio.

Two channels tagged `out-of-scope` before the `media` category existed were then
retagged `media`: Nuestra España Noticias (a general news outlet that covered the camps)
and Geoestrategia y Política (a one-person commentary channel; its camp posts are
supportive commentary rather than calls to action, so `media` rather than `ally`).

Project after the review: 132 channels — 22 `in-scope`, 79 `ally`, 29 `media`,
2 `out-of-scope` (Roto2bot, a forum-thread bot, and MEME_CCC, a meme channel).

## Decisions that needed judgement

- **Malditaultraderecha → `ally`.** 67 camp posts; it publishes calls ("Mañana ocupemos
  las plazas por todas las Maricarmen") and statements received from collectives.
- **Malditaultraderecha chat → not added.** 17 camp messages from 8 participants;
  individual chatter, some of it sceptical of the camp.
- **Revolución Comunista → not added.** Its 18 camp posts are reposted headlines and
  X posts; no voice of its own.
- **Diario Socialista → `media`.** It is the newspaper of Movimiento Socialista, whose
  youth organisation (Coordinadora Juvenil Socialista) is an `ally` with an empty
  channel. Tagged by kind, but it is the main Telegram voice of that current.
- **Movement agendas → `ally`.** Convocatorias Madrid, Convócala Málaga, Convocatorias
  Cádiz and Sevilla en Acción publish calls rather than news, so they are treated as
  movement channels, not media.
- **Publishers and periodicals of political currents → `media`.** Traficantes de
  Sueños, Tierra y Libertad, Viento Sur, Poder Popular, Regeneración and similar.
- **Two relevant channels could not be added:** Difusión Asamblea de Vivienda Sevilla
  (housing, 11 forwards) and the group Acampada Plaça Ajuntament (the València camp).
  Both are private or without a public username.

## Limits

- Keyword counts miss posts that are only images or that name the mobilisation
  differently; a channel with zero hits may still have taken part.
- A single camp post passes the test; the log gives the count so a stricter threshold
  can be applied.
- Channels were not added by anything except this review: the pre-review list is saved
  as `channels.before-external-review.json`.

## Second round (2026-10-05)

Scanning the channels added in the first round brought 85 new channels into the graph.
All 85 were reviewed with the same evidence and rule; rows are marked `round = 2` in
the log.

| Decision | Channels |
|---|---|
| Added as `in-scope` | 2 (Acampada per l'habitatge, the Barcelona camp's channel; Sindicat Llogateres Mallorca) |
| Added as `ally` — organisations | 9 |
| Added as `ally` — aggregators | 3 |
| Added as `media` | 21 |
| Not added — no camp post | 46 (38 organisations or other, 8 media) |
| Not added — aggregators | 2 |
| Not added — unreadable | 2 |

Project after the second round: 167 channels — 24 `in-scope`, 91 `ally`, 50 `media`,
2 `out-of-scope`.

Decisions that needed judgement:

- **Commentary and info channels → `media`**, following the Geoestrategia y Política
  decision: España en Guerra, Fullblack161, Prima Linea, GlobalRevolution,
  Anarquismo & Antimilitarismo.
- **Aggregators that relay calls → `ally`:** Antifascistas, Mitxis na Galiza
  Antifascista, Presos Revolucionarios. **Aggregators that only repost → not added:**
  Notice (Todos con Rusia), FemiNews.
- **Grupo Ruptura → `ally` with a caveat.** It passes the engagement test, but its post
  is critical of the camp. The rule tests engagement, not stance.
- **elPlural.com → `media`**, although the channel is an unofficial mirror of the site.
- **False positives discarded:** Red Antiespecista Madrid (an animal-rights camp in the
  UK) and L'Àgora Es Queda Al Barri (a camp against its own eviction, on 14–15 October).

The graph export now carries each reviewed node's `category` and `review` decision, so
channels that were reviewed and not added are still labelled in the GEXF.

The review has not been repeated on the nodes brought in by scanning the second-round
additions.
