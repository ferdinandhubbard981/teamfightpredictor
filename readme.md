neural network that predicts whether a teamfight will be successful for you or not

inputs:
	- [championtype, level, gold based on items, xpos, ypos]
	- ... x 10 where the first 5 are team blue and last 5 are team red

outputs:
	- good
	- bad


workflow:
	- get full game data
	- write a scripts to detect when a teamfight occurs (start and end)
	- extract data from teamfight every second from start to end
	- train neural network with training data (tensorflow)
	- c++ script to extract data realtime and feed it to neural network