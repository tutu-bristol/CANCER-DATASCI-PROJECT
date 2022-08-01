# Architecture of a Deep Neural Network for cancer detection in histopathologic scans of lymph node sections

This repository contains my code contributed to a group data science project involving the use of the biggest dataset of cancer image scans to train an AI algorithm (Deep Neural Network) to predict a negative or positive cancer diagnosis. 


**Task: binary classification**

**Dataset: - PatchCamelyon (PCam) dataset (learn more: https://github.com/tutu-bristol/pcam)** 

**Model: Artificial Neural Network (ANN), see information on layers within network below**


_________________________________________________________________
 **MODEL SUMMARY**
 
 Layer (type) |               Output Shape      |        Param #   
=================================================================
 rescaling_1 (Rescaling)  |   (32, 96, 96, 3)      |     0         
                                                                 
 flatten_1 (Flatten)     |    (32, 27648)         |      0         
                                                                 
 dense_10 (Dense)        |    (32, 128)           |      3539072   
                                                                 
 dense_11 (Dense)        |    (32, 96)             |     12384     
                                                                 
 dense_12 (Dense)        |    (32, 64)           |       6208      
                                                                 
 dense_13 (Dense)        |    (32, 36)           |       2340      
                                                                 
 dense_14 (Dense)       |     (32, 24)           |       888       
                                                                 
 dense_15 (Dense)      |      (32, 16)          |        400       
                                                                 
 dense_16 (Dense)      |      (32, 9)          |         153       
                                                                 
 dense_17 (Dense)       |     (32, 60)          |        600       
                                                                 
 dense_18 (Dense)       |     (32, 20)           |       1220      
                                                                 
 dense_19 (Dense)       |     (32, 1)            |       21        
                                                                 
=================================================================
Total params: 3,563,286

Trainable params: 3,563,286

Non-trainable params: 0



______________________________________________________________
 **HYPER-PARAMETER TUNING RESULTS (OPTIMAL NUMBER OF UNITS FOR EACH LAYER)**
=================================================================

Trial 44 Complete [00h 00m 16s]
val_accuracy: 0.5117647051811218

Best val_accuracy So Far: 0.7160784602165222
Total elapsed time: 00h 07m 20s
INFO:tensorflow:Oracle triggered exit

The hyperparameter search is complete. The optimal number of units in 1st densely-connected
layer is **33** and the optimal learning rate for the optimizer
is 0.0001.


The hyperparameter search is complete. The optimal number of units in 2nd densely-connected
layers is **65** and the optimal learning rate for the optimizer
is 0.0001.


The hyperparameter search is complete. The optimal number of units in 3rd densely-connected
layers is **97** and the optimal learning rate for the optimizer
is 0.0001.


The hyperparameter search is complete. The optimal number of units in 4th densely-connected
layers is **97** and the optimal learning rate for the optimizer
is 0.0001.


The hyperparameter search is complete. The optimal number of units in 5th densely-connected
layers is **97** and the optimal learning rate for the optimizer
is 0.0001.


The hyperparameter search is complete. The optimal number of units in 6th densely-connected
layers is **97** and the optimal learning rate for the optimizer
is 0.0001.


The hyperparameter search is complete. The optimal number of units in 7th densely-connected
layers is **33** and the optimal learning rate for the optimizer
is 0.0001.


The hyperparameter search is complete. The optimal number of units in 8th densely-connected
layers is **97** and the optimal learning rate for the optimizer
is 0.0001.


The hyperparameter search is complete. The optimal number of units in 9th densely-connected
layers is **33** and the optimal learning rate for the optimizer
is 0.0001.



______________________________________________________________
BEST EPOCH FOR OPTIMAL MODEL IS 14
=================================================================
![image](https://user-images.githubusercontent.com/98823082/182143729-a73f588b-d2cf-4489-a369-06fdd9813d93.png)

______________________________________________________________
HYPERTUNED MODEL PERFORMANCE ON TEST DATA
=================================================================
loss: 0.5803 - accuracy: 0.7020
