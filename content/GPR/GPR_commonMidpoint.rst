.. _GPR_commonMidpoint:


Common Midpoint Survey
======================

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


Thus, **any point** on the hyperbola can be used to determine the top-layer velocity from a common mid-point survey.
And once :math:`V` is determined, the definition of :math:`t_0` can be used to obtain the thickness of the top layer.



