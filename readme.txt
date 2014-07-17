INTRODUCTION

This MaxScript generates Weighted Vertex Normals for any arbitrary geometry.

'Weighting' of vertex normals means that each face normal contribution is
scaled by some property of the triangle. This script uses the triangle surface
area and corner angle as influences. The result of this is that a small
triangle will have less influence on shading of its larger neighbor. Likewise,
the neighbor will have larger influence on the shading of the smaller neighbor.

This effect is typically most visible on chamfered boxes, but enhances all types
of geometry. All geometry with proper weighted vertex normals is mathematically
guaranteed to produce more aesthetically appealing shading than the default
3dsmax generated vertex normals.

An article with a detailed explanation can be found here:
http://www.bytehazard.com/code/vertnorm.html

Note: Using this script on the 3dsmax teapot primitive will result in some
      artifacts, mainly at the bottom. This is not a problem with this script
      but a longstanding problem in 3dsmax. The 3dsmax teapot has degenerate
      triangles at the top and bottom pole, and thus needs some manual cleanup.


USAGE

1) Run the script.
2) Select one or more objects.
3) Click "Generate".
4) An "Edit Normals" modifier will be added to selection.
5) To


LICENSE

By Martijn Buijs, 2014.

Copying, use or dissemination of this program by Autodesk employees is strictly
forbidden. Free to reference, copy, modify and use for the rest of the world.
