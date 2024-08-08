.. _seismic_survey_design:

.. Survey geometry
.. ***************

.. As a motivating example, consider the following two figures, showing typical reflection and refraction survey layouts.

.. .. figure:: ./images/reflect.jpg
..	:align: center

.. If seismic signals travel at higher velocity in the lower layer, then some of
.. the seismic energy travels along the interface, returning to the surface as a
.. "head wave" along a wave front similar to the bow wave of a ship (figure
.. below). These are refracted waves, and for geophones a long way from the shot
.. point, they represent the first arrival of seismic energy. In other words,
.. because head waves travel along the interface at the velocity of the "faster"
.. material, they eventually overtake the direct waves (green in the figure
.. below) traveling in the slower surficial materials.
.. 
.. .. figure:: ./images/refract.jpg
.. 	:align: center
.. 
.. Of course energy is both **reflected** and **refracted**, so ground motion
.. detected at a geophone is a caused by the combination of direct, refracted and
.. reflected energy arriving at the geophone's location. The different types of
.. energy are distinguishable only because they have traveled along different
.. pathways. Refraction surveying takes advantage of the fact that refracted
.. waves arrive before reflected energy, so long as the geophone is at a great
.. enough distance from the shot point.

Survey geometry
===============

Multichannel data collection
----------------------------

First consider the source-receiver geometry. The geometry can be "split
spread" in which case there is a central shot with receivers on both sides, or
a "single-ended spread" in which the receivers are always on one side of the
source. Split spreads are common in land surveys; single-ended spreads are
common in marine surveys.

.. figure:: ./images/split_and_single_spread.gif
	:align: center
	:scale: 110%

	Shot-detector configurations used in multichannel seismic reflection
	profiling .(a) Split spread, or straddle spread. (b) Single-ended spread
	[#f1]_

.. figure:: ./images/shot_gather_split_spread.gif
	:align: right
	:scale: 100 %   

.. <<editorial comment>> The original GPG had a "click to enlarge" feature for the shot gather. Should it be added?

A split spread seismic record is shown above. The seismic traces all belong to
a single source and hence this is referred to as a "Common Source Gather". The
first arrivals are direct or critically refracted arrivals. Reflection
hyperbolae from numerous boundaries are observed, right. The strong energy in
the triangular central portion is ground roll caused by surface waves. It
masks the reflection events.



.. [#f1] From Kearey, Philip and Micheal Brooks, '*An Introduction to Geophysical Exploration*'. 2nd ed. Blackwell Science: 1991. 
