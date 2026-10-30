# Mini-Workshop on World Models — photo assets

This folder holds the public photographs for the **Mini-Workshop on World Models** at Columbia University (October 29, 2026).

**Workshop page:** https://alab-columbia.github.io/workshops/world-models-2026/

## Where the photos go

```text
ALab-Columbia.github.io/
├── workshops/
│   └── world-models-2026/
│       └── index.html               ← website page
└── assets/
    └── workshops/
        └── world-models-2026/        ← YOU ARE HERE
            ├── README.md
            ├── speakers/
            │   ├── README.md
            │   ├── oumayma-bounou.jpg
            │   ├── stephen-tu.jpg
            │   ├── adam-block.jpg
            │   ├── yunzhu-li.jpg
            │   ├── rohun-agrawal.jpg
            │   └── ying-wang.jpg
            └── story/
                ├── README.md
                ├── photo-01.jpg
                ├── photo-02.jpg
                ├── photo-03.jpg
                └── ... (up to photo-30.jpg)
```

The .jpg files in the tree are **names to use when uploading**; they may not have been added yet.

## 1. Speaker portraits

Upload **one headshot per speaker** to the `speakers/` folder, using these **exact** names:

| Speaker | Filename |
| --- | --- |
| Oumayma Bounou (NYU) | `speakers/oumayma-bounou.jpg` |
| Stephen Tu (USC) | `speakers/stephen-tu.jpg` |
| Adam Block (Columbia) | `speakers/adam-block.jpg` |
| Yunzhu Li (Columbia; remote talk) | `speakers/yunzhu-li.jpg` |
| Rohun Agrawal (Columbia) | `speakers/rohun-agrawal.jpg` |
| Ying Wang (NYU) | `speakers/ying-wang.jpg` |

**No HTML edits are needed.** Once a file with the expected filename has been uploaded and GitHub Pages has published it, the corresponding speaker card will show the photo instead of the initials.

## Portraits currently used on the website

The following portraits were sourced from speakers' personal research pages or a research workshop page. The **exact `.jpg` filenames above still work**: uploading your own approved JPG with that name takes precedence over a fallback image.

| Speaker | Current image | Original source |
| --- | --- | --- |
| Oumayma Bounou | **Stored in this repository** at `speakers/oumayma-bounou.jpg` | https://oumayb.github.io/ (self-published `assets/img/profile_2026.jpg`) |
| Stephen Tu | **Stored in this repository** as `speakers/stephen-tu.png`, currently the fallback until `stephen-tu.jpg` is uploaded | https://stephentu.github.io/ (self-published `profile_photo.png`) |
| Adam Block | **Loaded from original website** until `adam-block.jpg` is uploaded | https://abblock.github.io/portrait.jpg |
| Yunzhu Li | **Loaded from original workshop website** until `yunzhu-li.jpg` is uploaded | https://deformable-workshop.github.io/icra2025/imgs/yunzhu.jpg |
| Rohun Agrawal | **Stored in this repository** at `speakers/rohun-agrawal.jpg` | https://rohunagrawal.github.io/ (self-published `assets/img/portrait.jpg`) |
| Ying Wang | **Loaded from original website** until `ying-wang.jpg` is uploaded | https://yingwangg.github.io/assets/img/headshot.jpg |

The speaker cards credit their photograph sources. **Publicly accessible does not necessarily mean free to redistribute**. Please confirm permission or reuse rights with the photographer/speaker when using any photo on a public website. You can replace any portrait with a workshop photo that you have permission to publish.

## 2. Photo story (talks, discussion, candid moments)

Upload workshop-event photos into the `story/` folder using consecutive, two-digit filenames:

```text
story/photo-01.jpg
story/photo-02.jpg
story/photo-03.jpg
story/photo-04.jpg
...
story/photo-30.jpg
```

The workshop page **automatically discovers these photos**, starting at `photo-01.jpg` and continuing until it encounters the first missing number. **Do not skip a number** (for example, if `photo-03.jpg` is absent, `photo-04.jpg` will not be displayed).

You do **not** need to edit `index.html` just to add or remove a consecutively numbered photo. Put the photos in your preferred display order; chronological order works well (opening talk → later talks → group discussion).

### Optional captions

The gallery uses automatic labels such as “Workshop photo 01.” To provide real captions, edit the `storyCaptions` object in `workshops/world-models-2026/index.html`:

```js
const storyCaptions = {
  "01": "Oumayma Bounou presenting",
  "02": "Stephen Tu presenting",
  "03": "Audience discussion"
};
```

Use the two-digit number as the key. The gallery lightbox displays the same caption.

## How to upload through GitHub

1. Open [the **speakers** folder](https://github.com/ALab-Columbia/ALab-Columbia.github.io/tree/main/assets/workshops/world-models-2026/speakers) or [the **story** folder](https://github.com/ALab-Columbia/ALab-Columbia.github.io/tree/main/assets/workshops/world-models-2026/story).
2. Choose **Add file → Upload files**.
3. Drag the appropriately named `.jpg` images into GitHub.
4. Commit the changes to `main` (or open and merge a pull request).
5. Visit the [workshop page](https://alab-columbia.github.io/workshops/world-models-2026/) after GitHub Pages publishes the update.

## Photo format & permissions

- Use real **JPEG (.jpg)** files, not HEIC/HEIF, PNG renamed to .jpg, or `.jpeg`. File and extension names are case-sensitive.
- Prefer clear, landscape-oriented event photos and portrait-oriented speaker headshots. Roughly **1200–2000 px** on the longest side is plenty for the website; compress large files before uploading.
- Avoid spaces, accents, uppercase letters, and extra suffixes in filenames.
- The repository and GitHub Pages website are **public**. Only upload photos you have permission to share publicly.
- If a speaker portrait is unavailable, their initials stay visible; if there are no story photos, the “Photo story coming soon” placeholder stays visible.

The website source file is `workshops/world-models-2026/index.html`.
