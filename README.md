#VertexAngleCalculator
This transformer takes as input a line or a polygon and calculates the change of direction (angle) at each vertex.
Transformer inspired from VertexAngleCalculator (VICREA).
#Usage
This transformer takes as input a line or a polygon and calculates the change of direction (angle) at each vertex.

The resulting angles are stored in degrees [-180, + 180]. The value is set to 0 for the first and last vertex of an open line. Negative values represent a left turn following the direction of the geometry.

#Input Ports
**Input:** Lines and polygons to be processed.

#Output Ports
**Measures:**  Processed features. Resulting angles stored as a measure on each vertex.

**Vertices:**  Individual vertices with all original feature attributes. The resulting angle is stored in a variable. A sequential vertex identifier is also provided (_id.vertex). 

#Parameters
**Destination Measure Name:** identifies the name of both the measure and the variable in which the results are stored.

#Limitations
The transformer only supports fme_line, fme_polygon and fme_donut geometry. 
