# Artifical_Intelligence_Wiki

### :smiley: Artificial Intelligence

***Aritifical Intelligence***: Any techniques that enable computers to mimic human behavior.<br>
***Machine Learining***: Subset of AI that use statisticual methods to learn from data, identify patterns and make decisions. <br>
***Deep Learning***: Subset of ML that is based on artificial neural networks.<br>

Manufacturing, retailing, transporation, finance, healthcare, and virtually every other industry is taking advantage of AI to transform thier core process and business models. The effects of AI will be maginified in the coming decade. <br>

Constructing machine learning models requries domain knowledge, mathematical expertise, and computer science skill.

### :star: Standard Machine Learning Process
1. Identify business problems
2. Collect data from various resources
3. Lable target (Supervised machine learning)
4. Extract features that will be used as the input to train models
5. Partition data into training, validation and holdout data.
6. Determine model evaluation criteria
7. Train model
8. Analyze model outcomes / model selection
9. Deploy model

### :boom: Big Data
Big data refers to volume, velocity, and varity of data that is available.
* Volume: the amount of data immense.
* Velocity: the speed of data
* Variety: the different types of data, strucutre, as well as, unstructured

### Key Terminology
- Labels: things (y) we predict.
- Features: input variable (x)
- Models: define the relationship between labels and freateures.
  - Training: create the model
  - Inference: apply the trained model to unlabeld examples
- Regressin: predict continuous values
- Classification: predict discrete values

### Linear Regression
<p> y' = b + w1x1 (y': predicted label, b: bias, w1: weight, x1: feature) </p>
<p> In supervised learning, a ML algorithm builds a model by examining historical records and attempting to find a model that minimizes loss. --- empirical risk minimization. </p>
<p> Loss is the penalty for a bad prediction, which is a number indicating how bad the model is in terms of the prediction.</p>
<p> The square loss = the square of the difference between the label and the predcition </p>
<p> Mean square error = average square loss per record over the whole dataset </p>

## An iterative approach














### Classification
Classification is a technique by which you determine to what group a certain observation belongs.

### Confusion Matrix
After training each classification model, the resulting confusion matrix shows how accurately the model categroized each record and where it might be making errors.

<img src = 'https://miro.medium.com/max/356/1*Z54JgbS4DUwWSknhDCvNTQ.png'>

### Cross-Validation
<p> Cross-validation is an extension of the training, validation, and holdout (test sets) process that minimise the sampling bias of machine learning models. </p>
<img src='https://3gp10c1vpy442j63me73gy3s-wpengine.netdna-ssl.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-22-at-1.22.04-PM.png'>
<p> With corss validation, the non-holdout data was split into five buckets, it is called '5-fold cross validation'. We then use one protion of the data for validation, and the remainder as training dataset. </p>
<p> After that, five iterations of a model is built based on the training data set and is tested with the validation dataset. Then compute the average performance of the model on each of the validation partitions. </p>
<img src='https://3gp10c1vpy442j63me73gy3s-wpengine.netdna-ssl.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-21-at-4.26.53-PM.png'>
<p> If the original validation partition is not representative of the overall population, then the resulting model may appear to have a high accuracy when in reality it just happens to fit the unusual validation set, causing you to implement a model that actually has poor accuracy when applied to future data. With cross-validation, you double-check how accurate your model is on multiple difference validation set, making sure it will generalize well to data you collect in the future. </p>

### Feature Engineering
<p> Feature engineering is the addtion and construction of additonal variables, or features, to imporve machine learning model peformance and accuracy. The most effective feature engineering is based on sound knowledge of the business problem.</P>
<p> <em> Coming up with features is difficult, time-consuming, [and] requires expert knowledge. - Andrew Ng, chief scientis of Baidu, co-chairman and co-founder of Coursera, and adjunct professor at Stanford Univrsity </em> </P>
<p><em>Example</em> <br>
  To most machine learning algorithms, dates are a string of unrelated numbers with no particular signifance. But with feature engineering, we can ientify which dates are Wednesday, and which days occurs immediately before or after public holidy. Feature engineering exposes this kind of 'common knowlege' and expands the number of pratical insights and business values a dataset can yield.</P>
  
 ### Feature Impact
 <p> Identify which features in a dataset have the greatest effect on the outcome of a machine learning model. </p>
 <p> In the age of big data, the size and dimension of dataset is astronomical. Assessing which pieces of information are most crucial allows analysts and business professionals to focus on the factors that matter the most, saving time and resources.
<p> Feature impact is used in both feature selection and target leakage</p>
  
 ### Feature Selection
 Getting rid of the features that don't add values to the analysis, reducing the chance of overfitting, reducing the CPU, I/O, and RAM load, and increasing the models'interpretablity.
