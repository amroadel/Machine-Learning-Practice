An engineer at a power generation plant anticipates that power generated in the plant can be calculated only from ambient variables of the plant i.e. without knowledge of the machines and their efficiencies. He has data of ambient variables and electricity generated for several days, so to check if his anticipations are correct he asks you to predict Net daily generated electrical energy (E) MW for 200 days. 

The ambient variables of the power plant are:

1- Temperature (T) in °C

2- Ambient Pressure (P) in millibar

3- Relative Humidity (RH)

4- Exhaust Vacuum (V) in cm Hg

The training data includes ambient variables along with Net daily electrical energy (E) MW.


The variables are given without normalization.

This Problem is from Hackerearth: https://bit.ly/2WHgHof

To solve this problem, I used linear regression and minimized the cost function using gradient descent. Because the provided data was not normalized, I had to normalize it using 
the mean and standard deviation in order to help the gradient descent obtain a fast solution to the problem with a few number of itterations. Another way of minmizing the cost function 
is using the optimize.minimize() function from scipy library. 
