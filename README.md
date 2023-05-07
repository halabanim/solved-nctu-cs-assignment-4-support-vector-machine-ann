Download Link: https://assignmentchef.com/product/solved-nctu-cs-assignment-4-support-vector-machine-ann
<br>
<h2 data-id="Competition">Competition</h2>

This homework is held on <strong>Kaggle</strong> as a competition so that you could see how it works.

<ul>

 <li>Click the <strong><a href="https://www.kaggle.com/t/48def01d57064db7a397e85eb5c0dc30">link</a></strong> to participate.</li>

 <li>The competition provides you a training and a testing set.

  <ul>

   <li>training set – train.json</li>

   <li>testing set – test.json</li>

  </ul></li>

 <li>Since it’s a competition, you won’t know the answer to the testing set, which is for you to predict and submit.</li>

 <li>The standard procedure of a competition:</li>

</ul>

<ul>

 <li style="list-style-type: none;">

  <ol>

   <li>Understand the data</li>

   <li>Split the provided training set into <strong>training subset</strong> and <strong>validation set</strong> for validation methods.</li>

   <li>Preprocessing, model construction, tuning</li>

   <li>Retrain the best model with as much data as possible, and predict <strong>testing set</strong> and make a submission.</li>

   <li><span style="text-decoration: line-through;">Win the competition</span></li>

  </ol></li>

 <li>If you have any questions, post them in the <strong>Discussion</strong> section or on Discord so everyone can see and understand.</li>

</ul>

<h2 data-id="Objective">Objective</h2>

<ol>

 <li>Data Input – 5%

  <ul>

   <li>Download the training set and testing set from <a href="https://www.kaggle.com/c/2020-nctu-ml-hw4/data">Kaggle</a>.</li>

  </ul></li>

 <li>Data Preprocessing – 15%

  <ul>

   <li>Transform data format and shape so your model can process them.</li>

   <li><strong>Shuffle the data</strong>.</li>

   <li>Any data augmentation that can boost your final results. – 10%</li>

  </ul></li>

 <li>Model Construction – 50%

  <ul>

   <li>Support Vector Machine – 20%

    <ul>

     <li>for SVM model, you may want to try out different types of kernels and compare the result.</li>

    </ul></li>

   <li>Artificial Neural Networks – 30%

    <ul>

     <li>for ANN model, you could use any <strong>Neural Network</strong> based model you want and implement it by yourself.</li>

     <li>Every framework (such as TensorFlow or PyTorch) is allowed.</li>

     <li>explain the reasoning of your model choice, data augmentation, and training process.</li>

    </ul></li>

   <li>Validation method

    <ul>

     <li><a href="https://en.wikipedia.org/wiki/Cross-validation_(statistics)#Holdout_method">Holdout validation</a> with the ratio <span data-mathml="<math xmlns=&quot;http://www.w3.org/1998/Math/MathML&quot;><mn>7</mn><mo>:</mo><mn>3</mn></math>">7:37:3</span></li>

    </ul></li>

  </ul></li>

 <li>Results – 10%

  <ul>

   <li>Obtain the performances of all experiment settings <strong>in tables</strong> by the following metrics:</li>

  </ul></li>

</ol>

<ol>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ol>

     <li>Confusion matrix</li>

     <li>Accuracy</li>

     <li>Sensitivity(Recall)</li>

     <li>Precision</li>

    </ol></li>

  </ul></li>

 <li>Comparison &amp; Conclusion – 10%

  <ul>

   <li>Also some feedback, anything you want to tell me.</li>

  </ul></li>

 <li>Kaggle Submission – 10% (+30%)

  <ul>

   <li>After the validation, now you have working SVM and ANN models.</li>

   <li>Retrain one of your best models with the whole train.json, predict test.json, and submit your y_test.csv to Kaggle.</li>

  </ul></li>

</ol>

<ol>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     <li>You can check sample_submission.csv for the submission format.</li>

    </ul></li>

   <li>Take a screenshot of the <strong>Leaderboard</strong>, highlight your name, and put it in the report.</li>

   <li>Top 10 in the <strong>final Private Leaderboard</strong> can get 30 bonus scores.</li>

  </ul></li>

</ol>

<strong>Note that you still need to submit your report and code to the newE3 system.</strong>

<h2 data-id="Data---Recipe-Ingredients-Dataset">Data – Recipe Ingredients Dataset</h2>

<ul>

 <li>The objective of the competition is to predict the category of a dish’s cuisine given a list of its ingredients.</li>

 <li>In the dataset, we include the recipe id, the type of cuisine, and the list of ingredients of each recipe (of variable length). The data is stored in JSON format.</li>

 <li>An example of a recipe node in train.json:</li>

</ul>

<ul>

 <li>{          “id”: 24717,·          “cuisine”: “indian”,·          “ingredients”: [·              “tumeric”,·              “vegetable stock”,·              “tomatoes”,·              “garam masala”,·              “naan”,·              “red lentils”,·              “red chili peppers”,·              “onions”,·              “spinach”,·              “sweet potatoes”·          ]·          },</li>

</ul>

<ul>

 <li>In the test file test.json, the format of a recipe is the same as train.json, only the cuisine type is removed, as it is the target variable you are going to predict.</li>

</ul>