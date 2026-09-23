Stroke is common, and those who survive a stroke are often left with language impairments, or aphasia. There are thought to be around 400,000 people with post-stroke aphasia in the UK alone. This project is part of work designed to fill a gap in current medicine, which cannot predict who will recover from these deficits.

An early description of the problem is here: https://www.sciencedirect.com/science/article/pii/S2213158213000260

Naturally, the data associated with this code are private, so cannot be shared. The code expects a set of 3D brain images, plus .csv files containing tabular information including lesion load variables and non-lesion factors. The code expects the dataset to be cross-sectional: i.e., one 'row' per patient, and every row a unique patient. My data were shaped as follows:

Images: 1239 x 91 x 109 x 91 (i.e., 1239 patients, 91 x 109 x 91 voxels, 1 channel)
Demographics: 1239 x 7 tabular
Lesion load variables: 1239 x 396 (i.e. binary lesion images over-laid on 396 anatomically defined brain regions, acquired from public databases).
Language outcome variables: 1239 x 34 scores assigned by speech and language therapists
