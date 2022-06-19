# Food Name Entity Recognition 
Download the 'NER Annotator' from this link https://github.com/tecoholic/ner-annotator. It's free software to preprocessing your custom NER data and feed to Spacy model. It's very simple to preprocess your data. Here is given some step to preprocess:
Suppose my Food dataset in text file like,

# Dataset
Revani is a dessert that emerged with the cuisine of the Ottoman Empires.
Hummus is probably one of the best-known Middle Eastern foods.
Falafel is a dish originating from the Levant.
Baba ghannouj is a popular appetizer made from eggplant and tahini.
Knafeh is a buttery, crunchy dessert.
Red Wine is for gentleman.
Girls love strawberries.
Pumpkin pie is a common dish for thanks giving dinner.
Don't wanna celebrate Christmas without turkey.
Ice Ice pops are must after dinner.
Lacchi is an Asian radiational food.
Peas are good for children.
Coconut is a great source for reducing dehydration.
There's no cinema night without pop corn.
Kababs were born on middle east.

# Using NER Annotator
Prepare this dataset for train the model using 'NER Annotator'. After preprocess this dataset it'll be JSON format. And the dataset look like

[['Revani is a dessert that emerged with the cuisine of the Ottoman Empires.\r',
  {'entities': [[0, 6, 'FOOD']]}],
 ['Hummus is probably one of the best-known Middle Eastern foods.\r',
  {'entities': [[0, 6, 'FOOD']]}],
 ['Falafel is a dish originating from the Levant.\r',
  {'entities': [[0, 7, 'FOOD']]}],
 ['Baba ghannouj is a popular appetizer made from eggplant and tahini.\r',
  {'entities': [[0, 13, 'FOOD']]}],
 ['Knafeh is a buttery, crunchy dessert.\r',
  {'entities': [[0, 6, 'FOOD'], [21, 36, 'FOOD']]}],
 ['Red Wine is for gentleman.\r', {'entities': [[0, 8, 'FOOD']]}],
 ['Girls love strawberries.\r', {'entities': [[11, 23, 'FOOD']]}],
 ['Pumpkin pie is a common dish for thanks giving dinner.\r',
  {'entities': [[0, 11, 'FOOD']]}],
 ["Don't wanna celebrate Christmas without turkey.\r",
  {'entities': [[40, 46, 'FOOD']]}],
 ['Ice Ice pops are must after dinner.\r', {'entities': [[0, 12, 'FOOD']]}],
 ['Lacchi is an Asian radiational food.\r', {'entities': [[0, 6, 'FOOD']]}],
 ['Peas are good for children.\r', {'entities': [[0, 4, 'FOOD']]}],
 ['Coconut is a great source for reducing dehydration.\r',
  {'entities': [[0, 7, 'FOOD']]}],
 ["There's no cinema night without pop corn.\r",
  {'entities': [[32, 40, 'FOOD']]}],
 ['Kababs were born on middle east.\r', {'entities': [[0, 6, 'FOOD']]}]]
 
