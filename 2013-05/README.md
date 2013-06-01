May 2013: Learn ray tracing with POV-Ray
========================================
Four years ago, I wrote [a simple ray tracer][JRT] in Java to render a
scene hard-coded in the source code. After writing this ray tracer, I
came to know about sophisticated ray tracing engines available for free
on the internet. POV-Ray seemed to be one of the most popular engines
and I decided to learn to use it. However, I never managed to devote
time to learning it in the last four years. Finally, in May 2013, I
decided to teach myself to do ray tracing with POV-Ray. This activity
consisted of learning the concepts required to write scene descriptions
for POV-Ray, and writing a new scene each day for 25 days in the month
of May 2013.

[JRT]: http://susam.in/files/code/ray-tracing/


Contents
--------
* [Introduction](#readme)
* [A scene a day](#a-scene-a-day)
  * [Balls and boxes](#balls-and-boxes)
  * [Transformed Boxes](#transformed-boxes)
  * [Marble Sphere in Rubber Torus](#marble-sphere-in-rubber-torus)
  * [Crystal Ball](#crystal-ball)
  * [Prisms](#prisms)
  * [Ripples](#ripples)
  * [Textures](#textures)
  * [Window](#window)
  * [Sky and Water](#sky-and-water)
  * [Soft Shadows](#soft-shadows)
  * [Focal Blur](#focal-blur)
  * [Pawns](#pawns)
  * [Glass Pawns](#glass-pawns)
  * [Globe](#globe)
  * [Saturn](#saturn)
  * [Planets](#planets)
  * [Moon](#moon)
  * [Canoe](#canoe)
  * [Eggs](#eggs)
  * [Glass of Water](#glass-of-water)
  * [Glass Grid](#glass-grid)
  * [Earth and Sky](#earth-and-sky)
  * [Glasses](#glasses)
  * [Kaleidoscope](#kaleidoscope)
  * [Dice](#dice)
* [Installation of POV-Ray](#installation-of-pov-ray)
* [POV-Ray commands](#pov-ray-commands)
* [Study URLs](#study-urls)
* [Progress log](#progress-log)
* [Conclusion](#conclusion)


A scene a day
-------------
01. ### Balls and boxes ###
    ![Balls and boxes][S01]

    This scene consists of three spheres and three boxes. The scene is
    illuminated by three point light sources.

    One light source is shining from the top right corner of the scene.
    This light source is behind the camera. This casts the shadow of the
    green box on the blue ball and that of the blue ball on the yellow
    one.

    Another one is shining from the left side of the scene. This light
    source is also behind the camera. This casts the smaller shadow of
    the red box on the blue ball, that of the green box on the orange
    ball and that of the blue ball on the pale pink box.

    There is a third light source at the bottom right corner of the
    scene. This light source is present slightly in front of the camera.
    This casts the longer shadow of the red box on the blue ball.

02. ### Transformed Boxes ###
    ![Transformed Boxes][S02]

    The white box is centred at the origin. The camera is placed 10
    units behind the origin. One light source is placed 10 units behind
    the origin, i.e. at the same place where the camera is. There is
    another light source shining from the top left corner of the scene.

    All boxes except the three boxes in the bottom-right quadrant of
    this image have the same dimensions as that of the white box.

    The red box is translated to &lt;2, 2, 2&gt;, i.e. 2 units left from
    the origin, 2 units above the origin and 2 units further away from
    the origin in the direction perpendicular to the image.

    The green box is translated to &lt;5, 5, 2&gt;, i.e. it has been
    shifted further way towards the top right corner. As a result we can
    see more of its left and bottom faces.

    The blue box is translated to &lt;5, 5, 5&gt;, i.e. it is placed 3
    units behind the green box. As a result it appears smaller than the
    green box.

    The yellow box is first rotated around z axis by 45° and then
    shifted left by 5 units

    The cyan box is first shifted left by 5 units and then the box is
    rotated around z axis by 45°. In the rendered image, it can
    be seen that the whole box as a whole orbits around the z axis due
    to the rotation and occupies a new place 45° away from the
    yellow box in this orbit.

    The length of the brown box is first doubled along x axis, then it
    is rotated 45° around y axis. As a result, the elongated face
    is rotated towards left. Then it is translated to a new position
    below the origin, a little further away towards the right.

    The pink box is first rotated 45° around y axis. Then it is
    scaled by a factor of 2 along x axis. As a result, the diagonal of
    the box running along x axis seems to be elongated. Finally, this
    box is translated and placed right below the brown box.

    The maroon box is first rotated along y axis by 45°. Then it
    is translated to a new position right below the pink box. Finally,
    it is scaled by a factor of 2 along the x axis. As a result, the box
    appears to have moved further along the x axis. Also, its diagonal
    along the x axis appears to be stretched.

03. ### Marble Sphere in Rubber Torus ###
    ![Marble Sphere in Rubber Torus][S03]

    There are two light sources in this scene: one where the camera is
    situated, and another on the left side of the scene.

    The sphere and the torus appear to be specular due to Phong
    highlighting. As a result, two bright shiny spots can be seen on the
    sphere as well. One spot is closer to the camera while the other one
    is on the left side of the sphere. These spots are due to the two
    light sources. Similar but fainter shiny spots can be seen on the
    torus as well. The specular highlights on the torus appear fainter
    because a less saturation value was used for the Phong highlighting
    was used for the torus.

    In addition to making the sphere specular, it has also been made
    slightly reflective. As a result, a faint reflection of the torus
    can be seen in the bottom hemisphere of the sphere.

04. ### Crystal Ball ###
    ![Crystal Ball][S04]

    There are two light sources in this scene: one at the centre of the
    ceiling and another at the top of the wall opposite to the camera.
    The walls are glossy, and thus reflect the scene slightly.

    There is a mirror on the wall opposite to the camera. The mirror has
    a wooden frame. The reflection of a door in the wall behind the
    camera can be seen in the wall opposite to the camera.

    There is a crystal ball placed on a wooden block. There are two
    other coloured balls lying on the floor.

05. ### Prisms ###
    ![Prisms][S05]

    The room in this scene is similar to the room in the previous scene.
    However, in this scene the floor is reflective instead of the walls.
    The balls are missing from this scene and there are two prisms
    instead on the wooden block. The reflection of the door behind the
    camera can be seen in the mirror on the wall opposite to the camera.

06. ### Ripples ###
    ![Ripples][S06]

    This scene contains a rubber tube floating on water. There are
    ripples on the surface of water. The ripples have been made slightly
    turbulent in order to make it look a little natural.

07. ### Textures ###
    ![Textures][S07]

    This scene contains a wooden block and spheres with various textures
    placed on the floor of a room. The block is made of pine wood. There
    is a ruby glass sphere placed on the block. There is a pink granite
    sphere placed between the mirror and the wooden block. The leftmost
    sphere is made of white marble. The one to its right is made of
    brown agate. The next sphere that looks dark is made of blue agate.
    The reflective sphere on the floor is made of aluminium. The
    rightmost sphere is made of red marble. The mirror at the back shows
    a reflection of the scene.

08. ### Window ###
    ![Window][S08]

    This scene shows light entering a room through a window. Isotropic
    scattering makes the light beam coming through the window visible.

09. ### Sky and Water ###
    ![Sky and Water][S09]

    This scene contains water and sky. The sky contains clouds and the
    water contains irregular ripples. The water reflects the sky.

10. ### Soft Shadows ###
    ![Soft Shadows][S10]

    This scene contains a few marble balls and metal rods placed on a
    wooden plank. The scene is illuminated by three area light sources.
    The area light sources cast soft shadows. The light sources fade
    away with distance. As a result, the scene at the top left corner of
    the image appears to be darker than the rest of the scene. The soft
    shadows and the fading light sources make this image seem quite
    photorealistic.

11. ### Focal Blur ###
    ![Focal Blur][S11]

    This scene contains six coloured balls lying on a tiled floor. The
    camera is focussed on the white ball at the centre. The shallow
    depth of field causes other balls to blurred.

12. ### Pawns ###
    ![Pawns][S12]

    This scene contains a white pawn and a black pawn placed on a
    chessboard. There are two light sources shining on the chessboard:
    one from the left side and one behind the chessboard.

13. ### Glass Pawns ###
    ![Glass Pawns][S13]

    This scene contains glass pawns placed on a glass chessboard.

14. ### Globe ###
    ![Globe][S14]

    This scene contains a globe placed on a glossy surface. The globe
    was created by wrapping a map of the earth around a sphere. The map
    used to create this globe can be found in the 'resources' directory.

15. ### Saturn ###
    ![Saturn][S15]

    This scene is an attempt to model Saturn along with its five
    prominent rings. The planet and the rings are drawn to scale.

    The innermost ring is the D ring. The next ring that appears to be
    translucent is the C ring. The next opaque ring is called the B
    ring. Then there is a gap called the Cassini Division. After this
    division, lies the A ring. The A ring contains a thin gap called the
    Encke Gap. The outermost thin ring is the F ring. The region between
    the A ring and the F ring is called the Roche Division.

    The shadow of the gas giant on the rings can be seen in the right
    side of this image.

16. ### Planets ###
    ![Planets][S16]

    This scene represents the models of the eight planets of our solar
    system. The sizes of the planets are to scale in this scene. Names
    of the planets from left to right: Jupiter, Saturn, Uranus, Neptune,
    Earth, Venus, Mars and Mercury.

17. ### Moon ###
    ![Moon][S17]

    This scene contains a waxing half moon. This scene was created by
    wrapping a map of the moon around a sphere and rotating the sphere
    in order to show the side of the moon that is visible from the
    Earth.

18. ### Canoe ###
    ![Canoe][S18]

    This scene contains a white canoe floating on water. The hull of the
    canoe has been modelled using ellipsoids. The hollow section of the
    hull has been modelled by removing smaller ellipsoids from a large
    ellipsoid that forms the outer surface of the hull of the canoe. The
    canoe contains three wooden seats. The water is slightly reflective.
    The water reflects the sky, and thus appears blue in colour. A
    distorted reflection of the canoe can be seen in the water.

19. ### Eggs ###
    ![Eggs][S19]

    This scene contains half a dozen eggs lying on a tiled surface. Each
    egg is modelled by combining halves of a prolate ellipsoid and a
    sphere. The ellipsoid is cut into two halves at the equator. One
    half is used to model the little end of each egg. The big end of
    each egg is formed using a hemisphere cut off from the sphere. The
    length of the semi-major axis of the prolate ellipsoid is 1.6 times
    that of its semi-minor axis. The tiled surface on which the eggs are
    kept are slightly glossy and reflective. Two fading area light
    sources have been used to illuminate the scene. One light source
    shines from the left side of the scene. The other light source
    shines from the camera.

20. ### Glass of Water ###
    ![Glass of Water][S20]

    This scene contains a glass of water. There is only one point light
    source in this scene shining from the left side. The water has been
    modelled as a material with refractive index of 1.33. The reflection
    of light by the water has been modelled using Fresnel reflection.

21. ### Glass Grid ###
    ![Glass Grid][S21]

    This scene contains a grid made of glass nodes and edges. Each node
    in the grid is spherical. Each edge is cylindrical. The edges
    connect adjacent nodes.

22. ### Earth and Sky ###
    ![Earth and Sky][S22]

    This scene shows the earth and sky meeting at the horizon. A faint
    fog can be seen near the horizon. The shadows of the clouds can be
    seen on the ground. A viewing angle of 90° has been used to model
    the camera.

23. ### Glasses ###
    ![Glasses][S23]

    This scene contains two glasses kept in a kitchen corner. The
    kitchen has tiled walls. A faint reflection of the window in the
    kitchen can be seen on the wall behind the wine glass. Light
    entering from this window illuminates the kitchen. There is another
    yellow light source attached to the top of the wall behind the
    glasses.

24. ### Kaleidoscope ###
    ![Kaleidoscope][S24]

    This scene shows the inside view of a kaleidoscope. The kaleidoscope
    is constructed using three rectangular mirrors placed at 60° angle
    to one another so that they form an equilateral triangle shaped
    empty space between them. The triangular empty space between the
    mirrors can be spotted by looking for the orange disc at the centre
    of this image. The pink, green and purple discs around this orange
    disc are placed at three corners of this triangle.

    There are a few more objects, such as coloured grains, little
    pyramids and pearls placed in this empty space. Multiple reflections
    of these objects can be seen in the three mirrors surrounding the
    empty space. The reflection of the empty space can be seen as faint
    dark triangles throughout this scene.

25. ### Dice ###
    ![Dice][S25]

    This scene contains three glass dice placed on a wooden surface. The
    scene is illuminated by three fading area light sources.

[S01]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene01.png
[S02]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene02.png
[S03]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene03.png
[S04]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene04.png
[S05]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene05.png
[S06]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene06.png
[S07]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene07.png
[S08]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene08.png
[S09]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene09.png
[S10]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene10.png
[S11]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene11.png
[S12]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene12.png
[S13]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene13.png
[S14]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene14.png
[S15]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene15.png
[S16]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene16.png
[S17]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene17.png
[S18]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene18.png
[S19]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene19.png
[S20]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene20.png
[S21]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene21.png
[S22]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene22.png
[S23]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene23.png
[S24]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene24.png
[S25]: https://github.com/susam/25d/releases/download/2013-05-raytracing/scene25.png


Installation of POV-Ray
-----------------------
The scenes above were rendered using POV-Ray 3.6 on a Debian system. The
steps below describe how POV-Ray 3.6 was installed.

1. Download POV-Ray 3.6 for Linux from
   <http://www.povray.org/ftp/pub/povray/Official/Linux/povlinux-3.6.tgz>.
   In case, the above URL becomes unavailable in future, a copy of the
   tarball can be obtained from
   <https://github.com/susam/25d/releases/download/2013-05-raytracing/povlinux-3.6.tgz>.
2. Enter the following commands to begin installation.

        tar -xvzf povlinux-3.6.tgz
        cd povray-3.6
        bash install -no-arch-check

3. Enter `U` to make a user level installation at a custom location.
4. Enter `~/povray` as the custom location to install POV-Ray.
5. Enter the following commands to view the version and help message of
   povray and its man page.

        ~/povray/bin/povray
        man -M ~/povray/man/ povray

6. Add the following line to ~/.bashrc.

        export PATH=$PATH:~/povray/bin

   Now povray can be executed and its man page can be seen from any
   directory simply by entering the following commands.

        povray
        man povray

The following errors were faced during installation:

1. On trying to install by executing `./install`, the following
   error was displayed:

        This machine does not seem to be a Linux PC.

   This error occurred because the script looks for `i?86*` or
   `athlon*` in the output of `uname -m`, but the output on my system
   was: `x86_64`.
2. On executing `./install -no-arch-check`, the following error
   was displayed:

        ./install: 1094: read: Illegal option -n

   This error occurred because the script is executed by /bin/sh
   by default. This was resolved by executing the script with bash.


POV-Ray commands
----------------
The following commands obtain the resources directory required to render
scenes 14 to 17. These commands should be run within the 2013-05
directory, so that the resources directory is created in the same
directory as the pov files.

    wget https://github.com/susam/25d/releases/download/2013-05-raytracing/resources.tgz
    tar -xvzf resources.tgz

The following is a list of commands that were executed to render various
scenes.

    povray -W960 -H720 scene01.pov
    povray -W960 -H720 scene02.pov
    povray -W960 -H720 scene03.pov
    povray -W960 -H720 +A0.0 scene04.pov
    povray -W960 -H720 +Q9 +A0.0 +AM2 +R5 -J scene05.pov
    povray -W960 -H720 +A0.0 +AM2 scene06.pov
    povray -W960 -H720 +A0.0 +AM2 scene07.pov
    povray -W960 -H720 +A0.0 scene08.pov
    povray -W960 -H720 +A0.0 +AM2 scene09.pov
    povray -W960 -H720 +A0.0 scene10.pov
    povray -W960 -H720 scene11.pov
    povray -W960 -H720 +A0.0 +AM2 scene12.pov
    povray -W960 -H720 +A0.0 scene13.pov
    povray -W960 -H720 +A0.0 +AM2 scene14.pov
    povray -W960 -H720 +A0.0 +AM2 scene15.pov
    povray -W960 -H720 +A0.0 +AM2 scene16.pov
    povray -W960 -H720 +A0.0 +AM2 scene17.pov
    povray -W960 -H720 +A0.0 +AM2 scene18.pov
    povray -W960 -H720 +A0.0 scene19.pov
    povray -W960 -H720 +A0.0 +AM2 +R5 -J scene20.pov
    povray -W960 -H720 +A0.0 +AM2 -J scene21.pov
    povray -W960 -H720 +A0.0 +AM2 scene22.pov
    povray -W960 -H720 +A0.0 +AM2 -J scene23.pov
    povray -W960 -H720 +A0.0 +AM2 scene24.pov
    povray -W960 -H720 +A0.1 +AM2 scene25.pov


Study URLs
----------
The following is a list of tutorials and articles I studied to teach
myself some elementary ray tracing with POV-Ray.

1. [The Online POV-Ray Tutorial: Introduction to POV-Ray and Ray-tracing][T1]
2. [The Online POV-Ray Tutorial: POV-Ray Basics][T2]
3. [The Online POV-Ray Tutorial: Creating Simple Scenes][T3]
4. [The Online POV-Ray Tutorial: Advanced POV-Ray Features][T4]
5. [4 tips to improve a simple POV-Ray scene][T5]
6. [Slope map tutorial][T6]
7. [How to Render Planets][T7]

[T1]: http://library.thinkquest.org/3285/tutorial/intro.html
[T2]: http://library.thinkquest.org/3285/tutorial/basics.html
[T3]: http://library.thinkquest.org/3285/tutorial/simple.html
[T4]: http://library.thinkquest.org/3285/tutorial/advanced.html
[T5]: http://warp.povusers.org/povtips/
[T6]: http://warp.povusers.org/SlopeMapTutorial/
[T7]: http://www.midnightkite.com/index.aspx?URL=PlanetRendering


Progress log
------------
The list below shows how much time I spent each day learning new
concepts, coding and tinkering to generate each scene. The values
displayed below doesn't include the time spent by the computer in
rendering the images.

    Day  Date        Time   Comment
    ---  ----------  -----  --------------------------------------------
    01   2013-05-01  2.0 h  Balls and boxes
    02   2013-05-02  1.0 h  Transformed Boxes
    03   2013-05-03  0.5 h  Marble Sphere in Rubber Torus
    04   2013-05-04  1.5 h  Crystal Ball
    05   2013-05-05  2.0 h  Prisms
    06   2013-05-06  0.5 h  Ripples
    07   2013-05-07  1.0 h  Textures
    08   2013-05-08  1.0 h  Window
    09   2013-05-09  1.0 h  Sky and Water
    10   2013-05-10  4.0 h  Soft Shadows
    11   2013-05-11  3.0 h  Focal Blur
    12   2013-05-12  2.5 h  Pawns
    13   2013-05-13  1.0 h  Glass Pawns
    14   2013-05-14  1.0 h  Globe
    15   2013-05-15  1.5 h  Saturn
    16   2013-05-16  1.0 h  Planets
    17   2013-05-23  1.0 h  Moon
    18   2013-05-24  3.0 h  Canoe
    19   2013-05-25  1.5 h  Eggs
    20   2013-05-26  2.0 h  Glass of Water
    21   2013-05-27  2.0 h  Glass Grid
    22   2013-05-28  1.0 h  Earth and Sky
    23   2013-05-29  4.0 h  Glasses
    24   2013-05-30  5.0 h  Kaleidoscope
    25   2013-05-31  3.0 h  Dice

    Total Time:     47.0 h

Conclusion
----------
I began this 25 day learning challenge on 1 May 2013 and completed it
successfully on 31 May 2013. There was a 6 day gap from 17 May 2013 to
22 May 2013 due to a trip to Goa and other personal activities. This
activity demanded about 1 hour 53 minutes per day on average.

Some prior knowledge of coordinate geometry was helpful in describing
some of the scenes. I found the POV-Ray scene description language
pretty simple and easy to learn. In these 25 days, I managed to learn a
number of useful features and concepts from online tutorials, articles,
available source code of POV-Ray scenes described by other POV-Ray
users, and managed to describe and render many simple scenes. However,
there were a lot of options, features, language directives, effects,
etc. that I could not find time for in these 25 days. These things can
be learnt in future by studying the official [POV-Ray
documentation][DOC].

[DOC]: http://www.povray.org/documentation/
