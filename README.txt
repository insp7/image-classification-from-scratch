Steps to run the python notebook 

In the same directory where the notebook is present -
i) Inside the folder 'Data' extract the dataset here
ii) Keep the feature_extractor.py and authenticator.py

---Parameters---
The trained parameters are stored in 2 files :
parameters_augmented.pkl
parameters_original.pkl

These files are pickle of list trained_parameters[], the structure of the list is:
trained_parameters = [W1,b1,W2,b2,WL,bL]
where L is the notation for the last layer.

The predict function directly takes this list as an input argument.
in order to run the predict function :
unpickle the file to a list object and use it directly

paramters = unpickle(filename.pkl)
predict(X_test,Y_test,parameters)