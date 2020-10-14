

CANCER DRUG STUDY

Soure data was presented in two .csv files:

    Mouse_metada, which included data for each mouse tested (249 total), its age (months), weight(g), and the drug regimen it was on. 
    Study_results.csv which included tumor volume (mm3) and timepoints tested (days) for each mouse

DATA EVALUATION The data was evaluated to provide various metrics as follows:
* Generate a summary statistics table consisting of the mean, median, variance, standard deviation, 
	and SEM of the tumor volume for each drug regimen. (tumor_stats_df, in code)

* Total Number of Timepoints for each drug trial. Results are displayed in bar plots 
	- Fig 1 - Timepoints Per Drug Regimen Barplot - Pandas and
	- Fig 2 - Timepoints Per Drug Regimen Barplot - Pyplot

* Gender breakdown of mice in the study
	- Fig 3 - Gender Breakdown Pie Chart - Pandas
	- Fig 4 - Gender Breakdown Pie Chart - Pyplot

* Statistical Distrubtion of final tumor volume for all four selected treatment regimens (Capomulin, Ramicane, Infubinol, and Ceftamin)
	- Fig 5 - Final Tumor Volume Distribution - Boxplot

* Tumor Volume vs. Timepoint for Selected Mouse (x401)
	- Fig 6 - Tumor Size vs Time - Line Chart

* Mouse Weight vs. Average Tumor Volume for the Capomulin treatment regimen.
	- Fig 7 - Average Tumor Size vs Weight - Scatter Plot, Linear Reg

* Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment. Plot the linear regression model on top of the previous scatter plot.


RESULTS DISCUSSION:

-Based on the number of timepoints per drug regimen, Capomulin and Ramicane had the most timepoints. Final 
	tumor volumes for these drugs were smallest, and the standard error of the means were relatively low 
	(approximately 0.32), compared to other drugs. This suggests that these drugs are effective in reducing 
	tumor volume and that the data is representative of population 0effects.  However, this conclusion is 
	limited because the reasons for fewer timepoints with the other drugs(i.e. stopping the drug sooner) 
	are not known.  
- The final tumor volumes of Infubinol and Ceftamin were generally higher than those of Capomulin and Ramicane.
- Average tumor size and increased mouse weight showed a strong positive correlation.  