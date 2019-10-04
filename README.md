# Instrument detector
Attempting to detect instruments in music samples.

For this, I'll be using the OpenMic2018 dataset by Eric J. Humphrey, Simon Durand and Brian McFee. The full dataset can be found on [Zenodo](https://zenodo.org/record/1432913), and the original writeup is located [here](http://bmcfee.github.io/papers/ismir2018_openmic.pdf).

# Notes

- Instead of VGGish, we can use OpenL3
- dataset contains +/0/- flags for instruments - what can I do about the 0 flags?
- baseline model is a Random Forest (see writeup above)
- some of the classes are very "niche" e.g. trumpet, versus others which are broader e.g. vocals
- objective: a model that can classify a music sample on its instruments (e.g. classes "drums", "trumpet", "vocals")
