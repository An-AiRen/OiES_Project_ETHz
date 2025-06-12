The file of code is constructed as:

-summer_household_energydata.csv
-winter_household_energydata.csv
-optimizer_complete.ipynb
-data_visualisation.ipynb
-result_visualisation.ipynb



+ Input Data

	``summer_household_energydata.csv`` and ``winter_household_energydata.csv`` record electricity usage profiles of appliances for summer and winter, respectively. As for appliances, the input data keeps track of non-flexible appliances (dishwasher and washing machine) and critical appliances. It also comprises the PV generation which is perceived as an ideal forecast, as well as the dynamic price.

+ Optimizer

  ``optimizer_complete.ipynb`` serves as the demand response controller to minimize the electricity bill. For each scenario, the implementation is made up of two blocks of code. The first code block formulates the optimization problem and runs the solver. The other block prints out the cost over a week and save the result into a csv file. Note that the code works for winter, one could change the input flow of the variable ``household`` from ``winter_household_energydata.csv`` to ``summer_household_energydata.csv``  so that scenarios in summer can be simulated.

  Results have already been stored in the subfolder ``output`` which will be used for visualization lately.

+ Visualization

  ``data_visualisation.ipynb`` makes plots for the raw input data and ``result_visualisation`` showcases optimized profiles for every scenario.

