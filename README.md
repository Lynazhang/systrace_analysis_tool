Systrace Analysis Tool
============
Systrace Analysis Tool provides a series of python scripts to help analyse systrace results for Android application smoothness.

##How to run?
###Get surfaceflinger and process trace flie
	1.Copy systrace result (html file) to current dir.
	2.Fill in the 'app_config.ini' config file with surfaceflinger PID and app related info.
	3.python get_surfaceflinger_and_process_trace.py
Surfaceflinger trace file ends with '_surfaceflinger_trace.txt' and process trace flie ends with '_process_trace.txt'.
###Get FPS
	1.Fill in the 'fps_config.ini' config file for calculating FPS.
	2.python get_fps.py
FPS result pretents in output file ( end with '_fps_result.txt').
###Get performTraversals time list and frequency
	1.Fill in the 'performtraversals_config.ini' config file to get 
    performtraversals time and results.
	2.py get_performtraversals_frequency_and_time.py
Result presents in file ( end with '\_performtraversals_' + minimum_time + '.txt'), and includes follows.
	*All performTraversals function start time and cost time list during given time.
	*Total performTraversals function number.
	*Frequency for performTraversals function (/s).