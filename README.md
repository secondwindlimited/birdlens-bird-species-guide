# Bird Species Guide: 751 birds with scientific names and taxonomy (CSV)

**An open index of 751 bird species: common name, scientific name, order, family and genus, each linked to a full species profile with description, photos, calls and range.** Use it for birding checklists, quizzes, classroom projects, data science or as grounding data for AI.

Maintained by **[BirdLens](https://birdlens.secondwindltd.xyz/en)**, the AI bird identifier app. Point your phone at a bird or record its song and BirdLens tells you what it is in seconds.

📱 [BirdLens for iPhone](https://apps.apple.com/app/id6749273279) · [BirdLens for Android](https://play.google.com/store/apps/details?id=com.morningc.bird)

## What's inside

| File | Contents |
|---|---|
| [`data/species.csv`](data/species.csv) | 751 species: `common_name, scientific_name, order, family, genus, url` |
| [`SPECIES.md`](SPECIES.md) | The same index as a browsable page, grouped into 44 orders |

```csv
common_name,scientific_name,order,family,genus,url
American Goshawk,Astur atricapillus,Accipitriformes,Accipitridae,Astur,https://birdlens.secondwindltd.xyz/en/birds/fc84518ff2
```

## Quick start

```python
import pandas as pd

birds = pd.read_csv("https://raw.githubusercontent.com/secondwindlimited/birdlens-bird-species-guide/main/data/species.csv")
print(birds.groupby("order").size().sort_values(ascending=False).head(10))
```

## Identify a bird

- **By photo or by sound, instantly:** use the [BirdLens app](https://birdlens.secondwindltd.xyz/en).
- **By browsing:** open the [online bird guide](https://birdlens.secondwindltd.xyz/en/birds).
- **Lookalikes:** [House Sparrow vs Eurasian Tree Sparrow](https://birdlens.secondwindltd.xyz/en/birds/house-sparrow-vs-tree-sparrow).
- **Not sure which input to use?** Read [Bird identification by photo or sound](https://secondwindltd.xyz/guides/bird-identification-by-photo-or-sound/).
- **Organising field notes:** [bird identification features checklist](https://secondwindltd.xyz/tools/bird-identification-checklist/).

## BirdLens compared

- [BirdLens vs Merlin Bird ID](https://secondwindltd.xyz/comparisons/birdlens-vs-merlin-bird-id/)
- [BirdLens vs Picture Bird](https://secondwindltd.xyz/comparisons/birdlens-vs-picture-bird/)

## Why BirdLens

- **Two ways to identify:** a photo or a sound recording.
- **A field guide in your pocket:** species pages with descriptions, photos, calls and range.
- **Nearby species and identification history**, so every walk adds to your list.
- **Six languages:** English, Chinese, German, Spanish, Italian and French.

AI identification is a fast starting point. Check difficult birds against several field marks or with a local expert.

## License

The index in this repository: [CC BY 4.0](LICENSE.md). Use it anywhere, including commercially, as long as you credit **BirdLens** with a link to https://birdlens.secondwindltd.xyz/.

---

Made by [SECOND WIND LIMITED](https://secondwindltd.xyz/) · More open resources: [github.com/secondwindlimited](https://github.com/secondwindlimited)
