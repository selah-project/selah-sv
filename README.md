# Tanak — svensk återgivning (selah-sv)

Detta är en svensk återgivning av den hebreiska Tanak. Varje vers ligger
i en egen fil, och varje ord är bundet till sitt hebreiska original.

**Skrift: latinsk med svensk diakritik.** Texten är skriven på
rikssvenska.

## Filernas form

```
<bok>/<kapitel>/<vers>.json
```

Varje fil:

```json
{
  "translation": "versen i löpande text",
  "tokens": [{"surface": "hebreiskt ord", "gloss": "svensk betydelse"}]
}
```

`surface` — det hebreiska protokollet. Det är inte vårt att skriva; det
kommer från originalet och ändras inte.

`gloss` — den svenska betydelsen av **just detta** hebreiska ord. Antalet
glosor är lika med antalet hebreiska ord. Alltid.

`translation` — samma vers läst i ett sammanhang, så att den kan läsas
högt.

## Vad tecknen ⟨ ⟩ betyder

De används till två saker, och det är viktigt att hålla isär dem.

**1 · ⟨את⟩ — ett hebreiskt tecken som inte översätts.** Ordet את står
före satsens objekt. Svenskan har ingen motsvarighet, och därför låter vi
det stå som det är skrivet. Det är inget sättningsfel; det är ett ord som
faktiskt står i texten.

**2 · ⟨ord⟩ — svenska som hebreiskan inte har.** Hebreiskan utelämnar
ofta verbet *vara*. Där svenskan behöver det för att satsen ska hålla
sätts det inom tecknen: `Saligt ⟨är⟩ ⟨det⟩ folk`. Tecknen säger: *detta
ord har översättaren lagt till, det står inte i hebreiskan.*

**Inom tecknen står aldrig ett främmande språk.** Inuti ⟨ ⟩ står svenska
eller det hebreiska tecknet — inget tredje.

## Namnen

Guds Namn **översätts inte, det translittereras**.

| hebreiska | här | vad vi har avvisat |
|---|---|---|
| יהוה | **Jahve** | **HERREN**, **Herren**, **Jehova** |
| אלהים | **Elohim** | **Gud** på Namnets plats |
| אל | **El** | "gud" som artnamn |
| אלוה | **Eloah** | — |
| אדני | **Adonaj** | **Herren**, **Herre Gud** |
| שדי | **Shaddaj** | "den Allsmäktige" |
| יה | **Jah** | — |
| צבאות | **Tsevaot** | "härskarornas" |
| שאול | **Sheol** | "helvetet", "dödsriket" |

**HERREN har hört hemma i den svenska bibeln i århundraden** — i Karl
XII:s bibel, i Folkbibeln, i Bibel 2000. Ändå står det inte här. Det är
en översättning av en *titel*, inte av Namnet; på den plats där texten
säger יהוה är det ett ord som döljer Namnet. Den som vill höra
traditionen finner den i varje annan svensk bibel. Här står det som är
skrivet.

Böjning är i sin ordning så länge stammen förblir hel: **Jahve, Jahves;
Elohim, Elohims.** Det som inte får ske är att stammen bryts. Jahve tar
aldrig bestämt suffix — inte *Jahven*.

## Allmänt *gud* och *herre* är i sin ordning

Där hebreiskan talar om folkens gudar eller om en mänsklig herre står här
litet *gud*, *gudar*, *herre* — det är inte att dölja Namnet, det är
översättning. Det hebreiska tecknet avgör, inte det svenska ordet i sig.
I 1 Kungaboken 20:23 talar arameerna om sina gudar; **gudar** står där
med rätta.

## Hela regeln

Disciplinen som denna text har vuxit fram efter finns nedskriven i
Selahs huvudförråd: `docs/methodology/translation-discipline/sv.md`.

## Läge

Hela Tanak: **23 213 verser**, alla 39 böcker. Den hebreiska grunden är
OSHB / WLC 4.20.

Denna text är **en första genomgång**. Den är inte det sista ordet; den
är ett vittne. Läs den bredvid hebreiskan.

Hur texten kom till — och vad som gick fel på vägen — står i
`PROVENANCE.md` (på engelska). Arbetsanteckningarna står i `NOTES.md`.

## Licens

Creative Commons Attribution-ShareAlike 4.0 International. Se
`LICENSE.md`.
