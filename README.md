Artiste
=======

Artiste is a collection of static methods for creating `Path` objects initialized with different shapes.

<img src="https://raw.githubusercontent.com/mattlogan/Artiste/master/github_assets/artiste_shapes.png" width="350"/>

## Add as Dependency

Artiste is on jCenter.

```groovy
repositories {
    jcenter()
}
```

```groovy
dependencies {
    compile 'me.mattlogan.artiste:artiste:4.0.0'
}
```

## Overview

The `Paths` class contains the entirety of the public API for this library. It contains three static factory methods, including:

1. One method for creating a regular convex polygon.
2. One method for creating a regular star polygon.
3. One method for creating a circle.

## The API

```public static Path regularConvexPolygon(int left, int top, int right, int bottom, int numSides, float rotationDegrees)```

Creates a regular convex polygon Path.

 * **Parameters:**
   * `left` — Left bound
   * `top` — Top bound
   * `right` — Right bound
   * `bottom` — Bottom bound
   * `numSides` — Number of sides
   * `rotationDegrees` — Degrees to rotate polygon
 * **Returns:** A Path corresponding to a regular convex polygon.

```public static Path regularStarPolygon(int left, int top, int right, int bottom, int numPoints, int density, float rotationDegrees, boolean outline)```

Creates a regular star polygon Path. 

 * **Parameters:**
   * `left` — Left bound
   * `top` — Top bound
   * `right` — Right bound
   * `bottom` — Bottom bound
   * `numPoints` — Number of points on star
   * `density` — Density of the star polygon (the number of vertices, or points, to skip when drawing a line connecting two vertices.)
   * `rotationDegrees` — Number of degrees to rotate star polygon
   * `outline` — True if only the star's outline should be drawn. If false, complete lines will be drawn connecting the star's vertices.
 * **Returns:** A Path corresponding to a regular star polygon.

```public static Path circle(int left, int top, int right, int bottom)```

Creates a circle Path.

 * **Parameters:**
   * `left` — Left bound
   * `top` — Top bound
   * `right` — Right bound
   * `bottom` — Bottom bound
 * **Returns:** A Path corresponding to a circle.

## License

```
The MIT License (MIT)

Copyright (c) 2014 Matthew Logan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
