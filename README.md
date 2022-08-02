# Neural Network Charity Analysis

![deep-neural-network-AI](https://user-images.githubusercontent.com/100856534/182459951-825276c3-13fe-4d49-9da2-8863e924eb61.png)

Image Source: https://bdtechtalks.com/2021/01/28/deep-learning-explainer/

## Purpose of Analysis

Alphabet Soup is an organization that wants to make investments in charitable organizations. I was tasked with using machine learning techniques, specifically naural networks, to review a dataset provided to see if those who apply for charitiable aid were succesful in their attempts. This was accomplished through getting the data cleaned to be able to use in a model that was trained using TensorFlow and the Neural Network Playground. 

## Results

### Data Preprocessing:

  **1) What variable/s are considered the target/s for your model?**
  
  The target of the model was the "Is_Successful" column. This column would indicate which of the organizations were able to get funding. 
  
  **2) What variable/s are considered to be the features for your model?**
  
  All other columns would be considered features, with exception of two columsn that were removed, such as "EIN" and "Name." 
  
  **3) What variable/s are neither targets nor features, and should be removed from the input data?**
  
  "EIN" and "Name" were removed from the dataframe. The two columns removed do not add any potenital benefit to the analysis. They are catagorical data that gave name and number to a certain charity orgnaization.
  
  ###Compiling, Training, and Evaluating the Model
  
  **How many neurons, layers, and activation functions did you select for your neural network model, and why?**
  
  With the original run through of the data, two hidden layers were provided with 80 nodes and 30 nodes provided respectively. THis provided close to 6,000 parameters within the model. Upon training the model and running it through 100 epochs, the accuracy was 72.5% rounded.
  
  ![original code](https://user-images.githubusercontent.com/100856534/182463296-c86ad637-41ff-49bd-9c4e-762a1713e2f9.png)

![original accuracy](https://user-images.githubusercontent.com/100856534/182463316-c624154f-9ee2-467a-afb1-76bde1ec32b8.png)

Upon using the Neural Network Playground, I ran several iterations of hidden layers and neurons to come to several different types of training for the model. Ultimately, I ran through five hidden layers in total and switched between 50 and 100 epochs for each. 

  **Three Hidden Layers**

    1) 50 Epochs

  ![three hiddeb kayers 50e](https://user-images.githubusercontent.com/100856534/182463658-3e7c4b4f-52f5-470f-82fb-934334e3afaa.png)

    2) 100 Epochs

![three hiddeb kayers](https://user-images.githubusercontent.com/100856534/182463694-fadae6f8-1b68-44fc-9e6f-81295582e6c0.png)

  **Four Hidden Layers**

    1) 50 Epochs

![Four Hidden layers 50e](https://user-images.githubusercontent.com/100856534/182463781-6b32b7c7-dee5-435f-8fef-994bedb77658.png)

    2) 100 Epochs

![Four Hidden layers](https://user-images.githubusercontent.com/100856534/182463821-e5f01ef0-fa7f-49c8-b99b-9d32c1259956.png)

  **Five Hidden Layers**

    1) 50 Epochs

![Five Hidden Layers 50 e](https://user-images.githubusercontent.com/100856534/182463877-066f5afd-2f03-4ba8-a803-77b8c4816bee.png)

    2) 100 Epochs

![Five Hidden Layers](https://user-images.githubusercontent.com/100856534/182463951-270b2317-5042-4d71-a1ab-e918753c5f54.png)


**Were you able to achieve the target model performance of 75%?**

Ultimately no, through all of the training iterations the best performance i could get for accuracy was 72.6% with using 4 layers at 50 epochs. 

**What steps did you take to try and increase model performance?**

I used differing hidden layers and epoch levels. I wanted to see if I was under or over training the model. I also used the online assistance of the Neural Network Playground to simulate the hidden layers and neurons I was going to use. 

## Summary

Overall, with the differing amount of iterations that I ran through with this analysis the accuracy did not change all that much. Before optimization of the code the accuracy was 72.5%. With adding in hidden layers and neurons per layer the greatest I coudl do was 72.6%, which improvement-wise is not noticable at .1%. 

I would suggest furthering the analysis through either binning certain columns to create smaller data clusters. Such as the Income column. Or scrapping neural networks with this dataset and using a RandomForest or AdaBoost analysis to see if that type of machine learning process would better fit the data provided. 
  
