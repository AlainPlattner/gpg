.. _GPR_commonMidpoint:


Common Midpoint Surveys
***********************

        .. figure:: images_new/GPR_common_midpoint.png
		:align: right
		:figwidth: 40%
	
		Common midpoint survey configuration.
		

For this configuration, the distance between the transmitter and receiver are changed for every reading.
However, the halfway point between the transmitter and the receiver is kept the same.
As we will show, common midpoint surveys are useful for determining the top-layer velocity and thickness.

From the survey schematic, we see that if the interface is approximately flat, the point of reflection is the same for all readings.
As a result, the signal from the reflected wave in the radargram should form a hyperbola.

.. figure:: images_new/GPR_example_buried_object_2.png
	:align: right
	:figwidth: 50%

	Geometry shown how radargram can be used to find propagation velocity.


Once again, the travel time for the radiowave signal is given by:

.. math::
	t = \frac{2 \sqrt{ x^2 + d^2 }}{V}


where :math:`d` is the thickness of the top layer and :math:`x` is the distance between the mid-point and either the transmitter or the receiver.
Once again by defining :math:`t_0 = 2d/V`, the top-layer velocity is given by:

.. math::
	V = 2 \sqrt{ \dfrac{x^2}{t^2 - t_0^2} }


Thus, the shape of the hyperbola can be used to determine the top-layer velocity from a common mid-point survey.
And once :math:`V` is determined, the definition of :math:`t_0` can be used to obtain the thickness of the top layer.





Ray Paths
=========

.. figure:: images_new/GPR_wave_paths_diagram.png
    :align: right
    :figwidth: 50%

    Radiowaves signals measured by a receiver for a 2-layer Earth.

Now that we understand the background theory, let's put it all together.
At :math:`t` = 0 s, the source (Tx) generates a pulse of radio waves.
As we can see on the right, there are many paths in which radiowaves can take in order to reach the receiver (Rx).
The propagation velocities, reflections and refractions can all be explained using the equations found above.
On the right, we have an example of a radargram, which shows the returning signal at increasing distances :math:`x` from the source.
Let us now try and explain the nature of each ray path.

Path 1: Direct Air Wave
-----------------------


.. figure:: images_new/GPR_radargram_2layer_example.png
    :align: right
    :figwidth: 45%
    :name: fig_gpr_2layer

    Radargram for a 2-layer Earth.


This was travels through the air in a direct line from the transmitter to the receiver.
Recall that in the air, radiowaves propagate roughly at the speed of light (:math:`c = 3.00 \times 10^8` m/s).
As a result, the direct air wave is **always** the first signal measured by the receiver.
The time it takes this wave to reach the receiver is given by:

.. math::
    t_{air} = \frac{x}{c}


The direct wave is shown in **red** on the radargram.
According to the above equation, the velocity of the air wave is 1 divided by the slope of this line.


Path 2: Direct Ground Wave
--------------------------

This wave travels along the surface interface at velocity :math:`V_1`.
Like the air wave, the ground wave also takes a direct path.
Because :math:`V_1 < c`, the ground wave arrives later than the air wave.
The time it takes for the ground wave to reach the receiver is given by:

.. math::
    t_{ground} = \frac{x}{V_1}

The direct ground wave is shown in **pink**.
Like the air wave, the direct ground wave velocity can also be obtained from the slope of the line.


Path 3: Reflected Wave
----------------------

The reflected wave travels through medium 1 at velocity :math:`V_1`.
Because it takes a longer path than the direct ground wave, it arrives later.
The time it takes for the reflected wave to reach the receiver is given by:

.. math::
    t_{ref} = \frac{\sqrt{x^2 + 4h^2}}{V_1}


The reflected wave is shown in **green**.
Unlike direct waves, the arrival time for the reflected wave is hyperbolic, which makes it distinguishable from other signals.
After sufficient distances (:math:`h \ll x`), the previous equation becomes approximately linear.
This portion of the curve can be used to estimate the velocity of the top-most layer.
Notice how the slope of the direct ground wave and reflected wave are parallel.


Path 4: Critically Refracted at Surface
---------------------------------------

In GPR surveys, this wave tends to not be dominant and it is not easily visible in :numref:`fig_gpr_2layer`. We will thus not discuss it here. Refracted waves play an important role in Seismic surveys. We discuss them in detail in that chapter. 
