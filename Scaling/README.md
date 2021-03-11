# Scaling

Scaling should be done for the input and output data! This is important, because it makes different scales comparable to each other.
Also, Neural Networks work with small weights, which only be usefull if the data is in a comparable range.


Import the needed packages

> from sklearn.preprocessing import StandardScaler, RobustScaler, MinMaxScaler

lets assume your data is called X_train/X_test and y_train/y_test


## StandardScaler

This is the most popular scaler.

It sets the mean of your feauters/targets to 0 and the standard deviation to 1

> scaler = StandardScaler() 
>
> scaler.fit(X_train) #searching for the mean and std
>
> X_train = scaler.transform(X_train) # applying it to the trainings data
>
> X_test = scaler.transform(X_test) # and the same transformation to the test data 

## MinMaxScaler

This sets the lowest value of every feature/target to 0 and the highest value to 1

> scaler = MinMaxScaler()  
>
> scaler.fit(X_train)
>
> X_train = scaler.transform(X_train)
> X_test = scaler.transform(X_test)

## RobustScaler

Not to popular scaler.

It sets the median of your feauters/targets to 0 and scales according to the quardile range

>scaler = RboustScaler() 
>
​> scaler.fit(X_train) #searching for the mean and std
>
> X_train = scaler.transform(X_train) # applying it to the trainings data
>
> X_test = scaler.transform(X_test) # and the same transformation to the test data 


