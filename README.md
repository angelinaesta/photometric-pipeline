# photometric-pipeline
To facilitate my research, I built a Python tool that cleanly automates end-to-end processing of TESS light curve data based on user-defined transit parameters. I designed it to streamline high-volume photometric analysis, support custom model integration, and output analysis-ready datasets — making detailed work faster, scalable, and more consistent.

To open and properly run this pipeline:

1) Ensure the following packages are installed or can be imported when running the tool: NumPy, MatPlotLib, PyPlot, LightKurve, ipympl, Pandas, AstroPy, AstroPy Units.
2) (also described when running the tool) In the same directory as where this code is running, make a text file titled pipeline_inputs.txt that contains the transit time of the primary star (in +24570000 BTJD), system period (in days), primary eclipse duration (in hours), transit time of the secondary star (in +24570000 BTJD), and secondary eclipse duration (in hours). For an example of how to format it properly, please see the sample pipeline_inputs.txt file in this repo.
