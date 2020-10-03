---
title: "Image stack versus volume cuboid"
featuredImage: "./todo.png"
date: 2020-08-17T10:00:00-0800
---

3D data can be surfaces or volumetric, where the latter is the 3D
analog of a 2D pixelated picture (read: raster image).  The topic here
is volumetric data, not surfaces.

The current project goal is to get The Allen's brightfield image stacks viewable
in [Neuroglancer[(https://github.com/google/neuroglancer). The Allen's data portal, brain-map.org,
has the stacks but not in a format that Neuroglancer reads. So the task
is to wrangle the data such that it can be viewed in Neuroglancer.

Seemingly, in neuroscientific experiments imaging data is usually collected
sequentially in plates which naturally can be serialized as image
files. TIFF seems to be a popular format. These plate images can and
are used in multiple context. Neuroglancer wants cuboids though, so 
that is what the data needs to be represented as.

SpaceTX => Precomputed cuboid
web friendly formats of JSON pointing to chucks of data (images or cuboids)


