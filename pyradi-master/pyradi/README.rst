
---------
Overview
---------

The PyRadi toolkit is a Python toolkit to perform optical and infrared computational radiometry (flux flow) calculations.

The toolkit is an extendable, integrated and coherent collection of basic functions, code modules, documentation, example templates, unit tests and resources, that can be applied towards diverse calculations in the electro-optics domain. The toolkit covers

  * Models of physical radiators (e.g., Planck's Law) and conversion between values expressed in different units.

  * Mathematical operations for radiometry (e.g., spectral integrals, spatial integrals, spectral convolution)

  * Data manipulation (e.g., file input/output, interpolation, spectral quantity conversions, reading Flir Inc PTW files)

  * Detector modelling from physical parameters: including single element detectors and staring arrays

  * 3-D noise analysis of image sequences

  * Modtran tape7 read functions

  * Graphical visualization(2-D and 3-D graphs) in compact format, including cartesian, polar, image and mesh plots.

  * Spectral variables are expressed in Numpy arrays to ease spectral operations and integrals.

The individual scripts in the toolkit is supported by examples, test cases and documentation. These examples are included at the end of each script in the `__main__`  section.  If you just run the script, the code will be executed and results will be available in graphs or text files.


   
Prerequisites
-------------

This  toolkit requires (current versions in brackets)  
Python (2.7.12 or 3.5.2),
Numpy (1.7 or later),
SciPy (0.13 or later),
Matplotlib (1.3 or later).
Mayavi (4.1) (only for Python 2.7) is required only for one file to do three-dimensional rendering, the rest of the toolkit works fine without Mayavi.


Status
------

This project is Production. Current content is tested, stable and usable. With time and active use the scope of the pyradi offering will grow and expand. 

The development is ongoing as and when new needs arise.  We are open for feature requests as well.

Documentation
--------------

Local API documentation in html and pdf format is available in the pradi installation directory, along the paths `doc/_build/html/index.html` and `doc/_build/latex/pyradi.pdf`. 

Online API documentation in html format is available
`here <http://nelisw.github.io/pyradi-docs/_build/html/index.html>`_.

Detailed tutorial examples on the application of pyradi are available online in these 
`notebooks <https://github.com/NelisW/ComputationalRadiometry#computational-optical-radiometry-with-pyradi>`_.

For a detailed theoretical background and many more examples see the book_ by CJ Willers. See also SPIE8543Pyradi_. 


    
Example application 
--------------------

A typical radiometry toolkit requirement (very much simplified) is the calculation
of the detector current of an electro-optical sensor viewing a target object through the atmosphere. 
The system can be conceptually modelled as  
comprising a radiating source with 
spectral radiance, an intervening medium (e.g. the atmosphere), a spectral filter, 
optics, a detector and an amplifier. The pyradi toolkit provides several classes and
functions to implement this model with minimal code.
An example solution is given in this script_ and is further explained with results in SPIE8543Pyradi_.

    
.. _script: https://github.com/NelisW/pyradi/tree/master/pyradi/examples

.. [notebooks]: https://github.com/NelisW/ComputationalRadiometry#computational-optical-radiometry-with-pyradi

.. [online]: http://nelisw.github.io/pyradi-docs/_build/html/introduction.html#example-application
   
.. [book] *Electro-Optical System Analysis and Design: A Radiometry Perspective*,  
   C.J. Willers, Volume PM236, SPIE Press, 2013. http://spie.org/x648.html?product_id=2021423
   
.. [SPIE8543Pyradi] *Pyradi: an open-source toolkit for infrared calculation 
   and data processing*,  SPIE Proceedings Vol 8543, Security+Defence 2011,  
   Technologies for Optical Countermeasures, Edinburgh, 24-27 September, 
   C.J. Willers, M. S. Willers, R.A.T. Santos, P.J. van der Merwe, J.J. Calitz, 
   A de Waal and A.E. Mudau.
   
