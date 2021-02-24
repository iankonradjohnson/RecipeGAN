# RecipeGAN

This is a large pet project that I worked on for a few months. For your viewing convenience, the Jupyter Notebooks in the pipeline are labelled according to the sequence they are run.

## Idea

The idea for the project was to create a Tabular Generative Adversarial Neural Network (TGAN) to create new recipes trained on recipes sourced from the internet. It also contains functionality to compute the nutrition data for each recipe using USDA official nutrition data and Natural Language Processing (NLP), and fuzzy logic for each ingredient in the recipe. 

## Content

The bulk of the project (Steps 1-3) involves cleaning data, standardizing the messy measurement data from the recipes, and computing nutritional data for each recipe. The last portion uses a TGAN to generate novel recipes based off our sourced and generated data.

## Data

Two main data sources were used to acheive a robust nutrition calculator using NLP. 

[USDA FoodDataCentral](https://fdc.nal.usda.gov/) - this large dataset contains every food registered with the USDA and the nutrition contents as well as the ingredients for food products. We use this to calculate the nutrition data for the recipe using NLP and fuzzy logic.

[AllRecipes](https://www.allrecipes.com/) - AllRecipes features a large database of user-generated recipes which we use to calculate nutrition data for each recipe and as training data in the TGAN

## Future Inquiries

This project is structured in such a way that there are a wide variety of addition use cases to build on what is currently written. Here is a list of possibilities:

* Using user ratings and popularity for recipes to analyze correlation between nutrition content (protein/fat/carb) ratios and tastiness.
* Linking with a food molecule database (such as [BittereDB](http://bitterdb.agri.huji.ac.il/dbbitter.php), find combinations of flavor molecules and how they influence user ratings and popularity for a recipe.
* Use a different approach other than TGAN to find ingredient combinations and create new recipes using this method.

## License
[MIT](https://choosealicense.com/licenses/mit/)


