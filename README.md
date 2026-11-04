# Bone Atlas

Learn every bone in the human body on an interactive 3D skeleton.

**Use it here: [samplesize1.com/tools/bone-atlas](https://samplesize1.com/tools/bone-atlas/)**

Made by [@samplesize_1](https://www.instagram.com/samplesize_1/) to learn all 206 bones for an n=1 experiment.

## What it does

- All 206 bones of the adult skeleton on a 3D model you can rotate and zoom
- Two levels: the 60 bone names (bones of the same kind share one name), or all 206 bones one by one
- The whole body or one region at a time: head, torso, arm, hand, leg or foot
- **Study**: step through the bones with the arrows, or click any bone to see its name
- **Practice**: find each bone; misses come back a few questions later until you get them right
- **Test**: every bone once, timed, no help, with your best score saved
- Hints on or off: everyday names like "Patella (kneecap)", or technical names only
- X-ray and peel modes to reach bones hidden inside others
- Voice commands to zoom ("left foot", "spine", "whole body") in Chrome, Edge and Safari
- English, French, Spanish, Portuguese (Brazil) and German, plus Latin: the official Latin bone names (Terminologia Anatomica) with the interface in English
- Progress and best scores stay in your browser: no account, nothing is sent anywhere

## Run it yourself

It's a plain web page with no build step. Browsers won't load the 3D model from a page opened straight from disk, so serve the folder with any static file server:

```sh
git clone https://github.com/SampleSize1/Bone-Atlas.git
cd Bone-Atlas
python3 -m http.server 8000
```

Then open http://localhost:8000.

| File | What it is |
| --- | --- |
| `index.html` | The whole app: markup, styles and code |
| `skeleton.glb` | The 3D skeleton |
| `three-bundle.js` | [three.js](https://threejs.org/) r169, bundled into one file |
| `progress.js` | Saves progress in the browser (localStorage) |

## Licences and credits

- **Code**: MIT, see [LICENSE](LICENSE).
- **3D model** (`skeleton.glb`): from [Z-Anatomy](https://github.com/Z-Anatomy/The-blend), based on [BodyParts3D](https://dbarchive.biosciencedbc.jp/en/bodyparts3d/desc.html) © The Database Center for Life Science, licensed [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). If you reuse or change the model, keep this credit and share it under the same licence.
- **three.js**: MIT, see [licenses/three.js.txt](licenses/three.js.txt).

## Updates and feedback

This repository is copied automatically from [samplesize1.com](https://samplesize1.com/tools/) whenever the tool changes, so edits made directly here would be overwritten. Found a bug or have an idea? [Open an issue](https://github.com/SampleSize1/Bone-Atlas/issues).
