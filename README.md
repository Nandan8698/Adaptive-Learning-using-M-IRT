# Adaptive-Learning-using-M-IRT
this repo can be used by anyone who wishes to build his own Adaptive Learning Engine


If you want a quick overview of what's available and you hate reading when it's not on the terminal, run

./start_mirt_pipeline.py --help

for an overview of the arguments


Generate Data
Data is generated with

./start_mirt_pipeline.py --generate


This constructs a bunch of students with fake abilities, a bunch of exercises with fake difficulties, and simulates those students doing those exercises. You can examine the generated data in

<PATH_TO_GUAC>/sample_data/all.responses


###Train a model

You can train a model on data with

./start_mirt_pipeline.py --train

By default, this looks at the place that generate writes - at sample_data/all.responses. If you're interested in using your own data, you can use

./start_mirt_pipeline.py --train --data_file <PATH/TO/YOUT/DATA>


