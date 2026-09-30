# Profile artwork

The active artwork uses a single ginger kitten character across the greeting,
coding, sleeping, astronaut and section-header illustrations. Keep the rounded
face, short paws and connected body proportions consistent when adding poses.

Animations are self-contained SVG with CSS keyframes. Positioning wrappers stay
separate from animated groups so rotation does not overwrite layout transforms.

The README selects `assets/static/` through `<picture>` when reduced motion is
requested. After editing an animated source, regenerate its static counterpart:

```sh
python scripts/build-static-art.py
```

Review both the still pose and multiple animation frames on light and dark
backgrounds. Keep technology icons and generated analytics separate from artwork.
