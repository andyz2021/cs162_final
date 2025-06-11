## CS 162 Project Code

### Before running

Make sure that you install all required packages. Use the command
```
source .venv/bin/activate
```
to activate the virtual environment with all needed packages.

### ai_detection.ipynb

You should be able to run this just by running all cells. Note that you will need the following files: 
```
ai_detection_model_final
tokenized_train_data
tokenized_val_data
```
If the tokenized datasets are not in the current directory, you will need to run some extra cells, as indicated in the notebook.
Additionally, ai_detection_model_final is our model weights for the best performing version of the model. 
Additionally, all of the validation datasets are included in the current directory, which is needed for the notebook to run correctly.


### how to run on hidden test set

To evaluate our model on the hidden test set, please run the notebook:
```
ai_detection_test_set.ipynb
```

Please make sure the test set is in the format of:
```
text: "sample text"
source: "human" or "ai"
```

This will evaluate our best model on the hidden test set. If you want to first train the model, run the notebook:
```
ai_detection.ipynb
```
Up until you successfully train the model, then save it to your file system. Then, run the:
```
ai_detection_test_set.ipynb
```
notebook, and just replace:
```
ai_detection_model_final
```
with whatever the name of the newly saved model is. 


