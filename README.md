# NeuralNetwork

Assignment 2:
Neural Networks

Submitted By:
Rakshitha Mahesh Kumar (RXM210063)
Jeevan Desouza (JXD210021)


Number of free late days used: 0

Listing of sources and assignments used in assignment:


Dataset File: Glass data set. Classification of glass types to 6 class.
https://drive.google.com/file/d/1zr0szmuuGoDyiCWef_KaDTTBUiRblSDv/view?usp=sharing


•	Multiple attributes are used in linear regression. 
•	Number of attributes used are 9.
•	"RI", "Na", "Mg", "Al", "Si", "K", "Ca", "Ba", "Fe"
•	Output attribute “Type”
 



Code Collab link:
https://colab.research.google.com/drive/1rcAYul2ZexJdJ0uBDichr5eV-yH0FohN#scrollTo=mJNeF1faS4me

Dataset link:
https://drive.google.com/file/d/1zr0szmuuGoDyiCWef_KaDTTBUiRblSDv/view?usp=sharing


Data Preprocessing:
1.	No null values were present in the given dataset.
2.	Duplicate rows were removed from the dataset.
3.	Using the Standard Scaler library, dataset is normalized.
4.	Convert the categorical data into numerical data.




Final Result:

Activation Fucntion
	Learning Rate	Epochs
	Number of Hidden Layers	MSE Train
	MSE Test	R2 Train
	R2 Test	Accuracy	Val_accuracy
relu	0.01	100	3	0.06324259	0.08797747	0.360636	0.22393	72.35	62.79
relu	0.01	200	3	0.06480	0.0811	0.3483999	0.25132	71.6	60.47
relu	0.1	100	3	0.0668	0.088	0.3296834	0.21296	70.59	62.79
relu	0.1	200	3	0.077	0.0826	0.3174	0.2633	68.82	62.79
tanh	0.01	100	3	0.066	0.090	0.3278	0.1947	72.35	58.14
tanh	0.01	200	3	0.064	0.081	0.3680	0.2650	72.94	60.47
tanh	0.1	100	3	0.0689	0.094	0.3111	0.1758	72.35	55.81
tanh	0.1	200	3	0.064	0.0899	0.3368	0.2000	72.94	62.79
sigmoid	0.01	100	3	0.0673	0.0848	0.34104	0.23401	72.35	60.47
sigmoid	0.01	200	3	0.0692	0.0914	0.32367	0.1927	72.35	58.14
sigmoid	0.1	100	3	0.0649	0.0834	0.36929	0.25327	75.29	62.79
sigmoid	0.1	200	3	0.077	0.0932	0.2632	0.1868	70.00	60.47
relu	0.01	100	2	0.064	0.070	0.4495	0.3463	72.94	76.74
relu	0.01	200	2	0.066	0.077	0.3662	0.2851	72.94	74.42
relu	0.1	100	2	0.063	0.077	0.4326	0.3050	74.71	65.12
relu	0.1	200	2	0.0618	0.070	0.4546	0.3534	75.88	74.22
tanh	0.01	100	2	0.055	0.0757	0.57888	0.3733	78.24	65.12
tanh	0.01	200	2	0.064	0.064	0.064	0.064	78.24	65.12
tanh	0.1	100	2	0.0591	0.067	0.067	0.4209	78.24	76.74
tanh	0.1	200	2	0. 0.0614	0.065	0.4828	0.4161	75.88	74.22
sigmoid	0.01	100	2	0.065	0.0753	0.3779	0.3122	72.94	69.77
sigmoid	0.01	200	2	0.0644	0.0694	0.41409	0.3582	74.12	76.74
sigmoid	0.1	100	2	0.055	0.071	0.5646	0.3966	79.14	67.44
sigmoid	0.1	200	2	0.0636	0.0705	0.4143	0.3417	75.29	72.09


From the above table, we can find the following set performs the best:
Activation Function: sigmoid
Learning Rate: 0.01
Number of Hidden Layers: 2
Epochs: 200
For this combination, we saw both accuracy and validation accuracy good.

Tanh also performed well for 2 hidden layers
 


Here we can see that the sigmoid activation function performs the best. And, as we increase the epochs, the error decreases and accuracy increases. So, we can say that a neural network performs best if the epochs are increased. We can also say that sigmoid activation function works best with this dataset.

Output Plot:

	 ![image](https://user-images.githubusercontent.com/22761519/177191866-b1ccd417-c2d2-4c01-bd0b-6b525a6ebae5.png)


Here we can see that the accuracy keeps on increasing with epochs.
This is for the set (Activation Function: Sigmoid, Learning Rate: 0.01, Epochs: 200, Number of Hidden Layers: 2).

