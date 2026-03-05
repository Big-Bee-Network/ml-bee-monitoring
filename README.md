# Bee Monitoring ML Project

## Branches

- **preliminary-research**: All research content, data, models, and analysis
- **ventura-milkvetch**: Clean branch for Ventura Milkvetch specific work
Switch to the appropriate branch:
```bash
git checkout preliminary-research    # For all research content
git checkout ventura-milkvetch       # For Ventura Milkvetch work
git checkout synthetic-data         # for creating synthetic training data


### Updates for synthetic training data
- down_sample_video.py: downsamples video to half the size
- spit_video_frames.py: splits video into single frames
- render_bee_views.py: uses 3D photogrammetry model to create multiple views of the bee. Currently there is an issue with a shadow from a lighting source that should be fixed. Requires Blender.
- autocrop_bee.py: Crops the output from render_bee_views.py to just pixels
- overlay_bees_random_scaled_rotated_limit10.py: creates a transparent overlay of the bee on the video images.

  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.16415880.svg)](https://doi.org/10.5281/zenodo.16415880)
