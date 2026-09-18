# PROVENANCE — how this rendering came to be

*Swedish (Svenska), chair 77. Lit 2026-09-17. Floor 23,213 verses.*

This is the record of how the text in this repository was produced and
what went wrong with it. A machine-assisted rendering has no standing
unless you can see how it was made, so this file says both.

---

## The approach

Every verse is rendered from the Hebrew of that verse, under a written
discipline — `docs/methodology/translation-discipline/sv.md` in the Selah
repository, itself written in Swedish. Six rules govern it: the Hebrew
token is the unit; the Name stays the Name; both truths of Deut 6:4; no
foreknowledge (Gen 22:1 does not know Gen 22:13); numbers and marks stay
put; the translator has no word of its own.

**The `⟨ ⟩` brackets do two different jobs.** `⟨את⟩` is the Hebrew
direct-object marker, which Swedish has no word for; it is left standing
so the reader sees it. `⟨ord⟩` is a word Hebrew did not write but Swedish
grammar requires — visibly marked, so you can always tell what the Hebrew
said from what the grammar needed.

## The fight on this chair is the Name

| Hebrew | here | rejected |
|---|---|---|
| יהוה | **Jahve** | **HERREN**, Herren, Jehova |
| אלהים | **Elohim** | **Gud** in the Name's place |
| אדני | **Adonaj** | Herren, Herre Gud |
| שדי | **Shaddaj** | "den Allsmäktige" as a substitute |
| אל | **El** | "gud" as a type-name |

HERREN is the word of four centuries of Swedish Bibles — Karl XII,
Folkbibeln, Bibel 2000 — set in small capitals precisely to mark that the
Name stands under it. It is the most over-trained word this chair knows.
Lowercase *gud / gudar* for the nations' gods and *herre* for a human lord
remain lawful; the census applies that distinction by the token's Hebrew
surface, never by spelling.

## The thermometer

Swedish's neighbours use letters Swedish does not have: Danish and
Norwegian `æ ø`, German `ß ü`. That is a character-level probe with no
vocabulary dependence. **`å` is shared by all three Scandinavian
languages and must never be flagged**; flagging it would be measuring our
own blindness.

**Full tree: zero `æ ø ß ü`.**

---

## The burn

The relay rendered 23,090 of 23,213 verses and moved on with a residue of
**123**. The residue showed the signature the Czech chair had shown the
same day: consecutive verse pairs.

The gleaning ladder walked the 123 through `[32000 8000 48000 4000 24000]`,
first success winning:

| ceiling | landed |
|---:|---:|
| 32,000 | 115 |
| **8,000** | **7** |
| 48,000 | 1 |

Seven seats landed only when the ceiling went **down**. Both failure modes
report the same `:json-error`; the verse length, not the status, says which
way to move.

## Finding: a success count that measured the wrong chair

The first attempt at the sv residue fed its 123 seats to the Czech chair's
re-press tool, which had `:lang :cs` hardcoded. It re-rendered **123 Czech
verses** over their cured state, left the Swedish seats missing, and
reported `{:ok 123}` while doing it. The only signal was that the Swedish
file count did not move.

The Czech corpus had been committed hours earlier, so it was restored
byte-for-byte and the bad renders were kept aside. The tool now takes the
language as an argument. **A success count says the calls succeeded, not
that they landed where you aimed them.**

## Finding: the corpus sat through a crash uncommitted

The session crashed with this corpus complete and cured but not yet in
git. It survived; it was committed at once (`5dd6224`). A chair's
repository is committed at seating, not after.

## The cure

The census came back structurally clean on the full tree: no JSON
errors, no empty flows, token rows or glosses, no row-count disagreements
with the floor, no corrupt Hebrew surfaces.

Four empty glosses no automated pass reaches were decided against the en
floor (`sv_hand_pass.clj`): the *-teen* half of two numerals (`-ton`), a
supplied particle at 1-samuel/1/6 (`⟨upp⟩`), and Aramaic's own object
marker `יתהון` at daniel/3/12 (`dem`, matching the floor while that
question is open).

## Finding: the erasure the census could not see

The census reads the token **rows**. The reader reads the **flow** — the
verse's running translation. A scan of the flows found **55** carrying a
bare erasure word, and in most of them the row was right while the flow
was wrong:

```
row:   האלהים → Elohims
flow:  … till staden där Guds man var.
```

`Guds man` — *man of God*, איש האלהים — stood seventeen times in the
flows against fifteen `Elohims man`. The row and the flow are two
surfaces; the cure had reached one of them.

`sv_name_pass.clj` cured **51** seats:

- **32** where the row was right and the flow erased — the flow takes the
  row's form (`Elohims man`, `Elohims berg`, `Elohims ark`). Six of these
  were written out by hand because the chair had doubled or bent the
  phrase (`Guds stav, Elohims stav` → `Elohims stav`).
- **5** where both surfaces erased the אלהים family.
- **12** involving אל, אדני, אדון: `Els berg` for הררי אל and for the altar
  hearth הראל; `mitt livs El` (Ps 42:9); `Ack, Adonaj` (Josh 7:8, where the
  row had given the plea בי the title *Herre*); Ps 136:2–3 returned to their
  rows (`Elohim över alla elohim`, `Adonaj över alla herrar`), dropping a
  commentary bracket the chair had added in its own voice.
- **2** further: the doubled `eder Eder Gud` at Josh 4:23, and a row at
  Ps 41:14 that had lost the Name entirely.

After the pass, five flows still carry a bare erasure word, all of them
held seats (below).

## Open — declared, not repaired

- **Aramaic** — ezra/5/17, ezra/6/5, ezra/6/16, daniel/6/17. D1 covers
  Hebrew only; there is no row to follow.
- **`Elohim ⟨Gud⟩`** — nine seats where the Name stands and the chair
  supplied a bracketed `Gud` beside it. Awaiting a ruling.
- **ית** — daniel/3/12. Thirty-one chairs mark Aramaic's object marker
  where the en floor does not.

## Final

**23,213 / 23,213 verses · 305,507 / 305,507 token rows.**
Jahve verses: **5,797**. Danish/Norwegian/German letters: **0**.
Licensed erasures remaining: **14**, every one a held seat above.
