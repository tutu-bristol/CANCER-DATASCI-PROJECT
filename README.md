# Architecture of a Deep Neural Network for cancer detection in histopathologic scans of lymph node sections

This repository contains my code contributed to a group data science project involving the use of the biggest dataset of cancer image scans to train an AI algorithm (Deep Neural Network) to predict a negative or positive cancer diagnosis. 


**Task: binary classification**

**Dataset: - PatchCamelyon (PCam) dataset (learn more: https://github.com/tutu-bristol/pcam)** 

**Model: Artificial Neural Network (ANN), see information on layers within network below**


_________________________________________________________________
 Layer (type) |               Output Shape      |        Param #   
=================================================================
 rescaling_1 (Rescaling)  |   (32, 96, 96, 3)      |     0         
                                                                 
 flatten_1 (Flatten)     |    (32, 27648)         |      0         
                                                                 
 dense_10 (Dense)        |    (32, 128)           |      3539072   
                                                                 
 dense_11 (Dense)            (32, 96)                  12384     
                                                                 
 dense_12 (Dense)            (32, 64)                  6208      
                                                                 
 dense_13 (Dense)            (32, 36)                  2340      
                                                                 
 dense_14 (Dense)            (32, 24)                  888       
                                                                 
 dense_15 (Dense)            (32, 16)                  400       
                                                                 
 dense_16 (Dense)            (32, 9)                   153       
                                                                 
 dense_17 (Dense)            (32, 60)                  600       
                                                                 
 dense_18 (Dense)            (32, 20)                  1220      
                                                                 
 dense_19 (Dense)            (32, 1)                   21        
                                                                 
=================================================================
Total params: 3,563,286
Trainable params: 3,563,286
Non-trainable params: 0
_________________________________________________________________
125/125 [==============================] - 1s 3ms/step - loss: 0.5670 - accuracy: 0.7180
