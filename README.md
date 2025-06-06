# photometric-pipeline
To facilitate my research, I built a Python tool that cleanly automates end-to-end processing of TESS light curve data based on user-defined transit parameters. I designed it to streamline high-volume photometric analysis, support custom model integration, and output analysis-ready datasets — making detailed work faster, scalable, and more consistent.

Inputs:
- eclipse times in .txt file (see details below)
- star ID
- desired customization and truncation details

Outputs (all lightcurves are clean, high-quality graphs):
- raw lightcurve
- SAP and PDCSAP lightcurves
- flattened lightcurve with and without transit masks
- folded and binned final lightcurve

# To open and properly run this pipeline:

1) Ensure the following packages are installed or can be imported when running the tool: NumPy, MatPlotLib, PyPlot, LightKurve, ipympl, Pandas, AstroPy, AstroPy Units.
2) (also described when running the tool) In the same directory as where this code is running, make a text file titled pipeline_inputs.txt that contains the items listed below. For an example of how to format it properly, please see the pipeline_inputs_sample.txt file in this repo. Items to include when making your own text file:
   - transit time of the primary star (in +24570000 BTJD),
   - system period (in days),
   - primary eclipse duration (in hours),
   - transit time of the secondary star (in +24570000 BTJD),
   - and secondary eclipse duration (in hours).
3) m

# To demo the software with the sample text file and confirmed information:

1)  Change the name of the sample file to pipeline_inputs.txt so the tool can read it in.
2)  When asked which object's lightcurves you would like analyzed, enter TIC 288878839
3)  Next, when choosing a number from the leftmost column, enter 1
4)  When asked for SAP or PDC flux, enter S
5)  
