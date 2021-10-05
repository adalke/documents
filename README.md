# Documents from Andrew Dalke

This is a place for me to put documents for others to find and read.

* [What's new in chemfp 4.0](WhatsNewInChemfp4.ipynb). Distributed to
customers on 1 October 2021 as part of the chemfp 4.0b1 "preview"
release. It gives a few examples of the new features in chemfp 4.0.

* [MolPort diversity scores vs. ChEMBL similarity scores](MolPortDiversity_v_ChEMBL_similarity.ipynb) - a short example showing how to use MaxMin to select 5,000 diverse
fingerprints from the 8M in MolPort, which are also diverse from the
260k fingerprints ASINEX Gold and Platinum. Then plot the diversity
score with the similarity of each fingerprint to its nearest of 2M
ChEMBL fingerprints. Takes about 14 minutes total.

* [k2Sweep](k2Sweep.ipynb) - a sweep-based heuristic to find a most
novel fingerprint in a dataset. "Most novel" means the Tanimoto score
between the fingerprint and its nearest neighbor is the smallest of
all nearest-neighbor scores. I place it in the context of MaxMin picking,
describe what sweep-search means, including 2Sweep and 4Sweep, show that
those standard graph methods don't seem useful for Tanimoto data sets,
and propose a variant which uses a number of nearest-neighbor searches
to select an improved initial pick.
