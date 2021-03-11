# Scaling

Scaling should be done for the input and output data! This is important, because it makes different scales comparable to each other.
Also, Neural Networks work with small weights, which only be usefull if the data is in a comparable range.


Import the needed packages

> from sklearn.preprocessing import StandardScaler, RobustScaler, MinMaxScaler

lets assume your data is called X_train/X_test and y_train/y_test


## StandardScaler

This is the most popular scaler.
It sets the mean of your feauters/targets to 0 and the standard deviation to 1.

> scaler = StandardScaler() <br>
> scaler.fit(X_train) <br>
> X_train = scaler.transform(X_train) <br>
> X_test = scaler.transform(X_test) <br>

## MinMaxScaler

This sets the lowest value of every feature/target to 0 and the highest value to 1.

> scaler = MinMaxScaler() <br>
> scaler.fit(X_train) <br>
> X_train = scaler.transform(X_train) <br>
> X_test = scaler.transform(X_test) <br>

## RobustScaler

Not to popular scaler.

It sets the median of your feauters/targets to 0 and scales according to the quardile range.

> scaler = RobustScaler() <br>
> scaler.fit(X_train) <br>
> X_train = scaler.transform(X_train) <br>
> X_test = scaler.transform(X_test) <br>

# Inverse Scaling

If you have scaled your data, used the algorithm, and got some predictions, you might want to scale everything back into the original space.
This can be done by:

> X_train = scaler.inverse_transform(X_train)

Be careful to that 'scaler' is actually the right scaler. Therefore it is good to give for scaler for the features another name than the target scaler.
