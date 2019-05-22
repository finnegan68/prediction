# Sales prediction 
Time series model is purely dependent on the idea that past behavior and price patterns can be used to predict future price behavior. A recurrent neural network deals with sequence problems because their connections form a directed cycle. In other words, they can retain state from one iteration to the next by using their own output as input for the next step. That's why i used LSTM.

As i had not very much time, here i want to describe some methods that can reduce RMSE.
1. Try different input sequence length. In my example i used just 28 days. 
2. Use grid/random search for parameter tuning. We need much for this methods, so i just changed the parameters manually.
2.1. RMSE on train set was lower than on test, so we should tune regularization or Dropout.
3. Use other ML algorithms. I used RNN because we talked about it on interview, and discussed similiar problem. But for this problem we can also try to use simple Linear Regression or some other algorithms.
4. Use cross validation / change size of test/train set.

