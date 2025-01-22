# whidbey_sunset_bay_hydrophones
Collect and process audio data from the sunset_bay hydrophone in the OrcaSound network

aws_sunsetbay_datasort.ipynb

- This file connects your local computer to the AWS Amazon buckets holding the data from Orcasounds hydrophones. You will need a CSV file holding the date and starting time of the recorded sections you would like download to your computer.

cable_layout_w_detections.ipynb

- This file will plot the cable coordinates and detections logged through Acartia.io, it will cross-correlate audio detections with visual detections and form a list of all audio detections that are logged within a certain buffer time of each visual detection. This requires using the bathymetry map which can be found in this repository as well.

hydro_spectro.ipynb

- This file takes the files created by the aws_sunsetbay_dataset.ipynb and processes them, generating PSDs, FFTs, and spectrograms to visualize the detections.

orcasound_entries.xlsx

- Use this file to model your own CSV file off of, or use this one to see how the code works!
