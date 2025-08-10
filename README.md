# I. Author's Context
I've held leadership roles in numerous VC-backed tech startups, but:
  - they were all __business__ roles (finance, COO, product)
  - I have no CS degree
  - have never undergone a coding bootcamp
<br>
After building some CRUD web apps and ETL pipelines, I'm upskilling in __Applied ML Engineering__. An ex-Google dev showed me an industry standard book by Aurelien Geron.

<br>
<br>

| CHAPTER | FOUNDATIONAL PROJECT         | TECH/MODEL USED                   | STATUS              |
|---------|------------------------------|-----------------------------------|---------------------|
| 2       | Predicting housing prices    | Supervised Learning, Regression   | Completed/published |
| 3       | Handwritten digits           | Image classification              | Completed/published |
| 4       | Training regression models   | Supervised Learning               | Completed/published |
| 5       | Classifying data points      | Support Vector Machines (SVM)     | Skipping            |
| 6       | Tree-based models            | Decision Trees, Random Forests    | Completed/published |
| 7       | Combining models             | Ensemble Learning                 | ** **This project** **         |
| 8       | Reducing dataset complexity  | Dimensionality Reduction          | Not Started         |
| 9       | Grouping similar data points | Clustering, Unsupervised Learning | Not Started         |
| 10      | Building neural networks     | Neural Networks, Deep Learning    | Not Started         |
<br>
<br>

# II. What is This?
So far, we've done basic regression models, basic classifiers, and basic decision trees. This project will be about:

- Random Forests
- Combining multiple methods

### Chronology of Topics
Consider that the data scientist/Applied Machine Learning Engineer is a handyman trying to build a house.

#### Chronology of Topics
- **Baseline (standalone) vs Ensemble Models**: Reviewing what we've learned in previous chapters, drawing context for how they inform ensemble learning
- **Bagging - Random Forest**: Demonstration of Random Forest with Taiwanese credit card company
- **Boosting and Stacking**: How this differs from Bagging 
- **Strategic Outcome**: What are we going to do with these findings, if anything?


# III. Major Learnings:
#### Data Availability
- It took way longer than I expected to find a suitable data set to work with. There were data sets with mystery titles, had zero documentation on what the feature labels, had too many blank values which nullified their use(no pun intended but seemingly forced), or the row count was too small support a meaningful analysis (particularly dangerous for Stacking)

- Sometimes the data you want isn't all in one source, and maybe it's possible to do a join, but then there's issues where anonymized data (like COVID or financial) prevents you from linking data sets

#### Off-Loading the Heavy Math Responsibilities
- It's astounding how far a novice can go with Scikit-learn doing the heavy lifting on math. Yes, I'm aware a human judgment and domain experience are needed for matters like feature engineering, feature elimination, and explainability. But I can see that you don't need to be a wizard inc college-level Calculus or Stats classes to get the general direction

#### Complaints Over Geron's Level and Other Teaching Materials On Social Media
- This book was recommended to me by someone who likely overestimated my starting point, and it didn't work for me that Geron just jumped right into the material without explaining the taxonomy like I did in my first notebook. I'm committed to finishing this out as a matter of self-discipline, but if I was to advise my younger self, I would have started with something easier before this textbook. Maybe if I 
   mprovements:
#### Sample Data Choices
- If I was to do this again, I would have picked a use case with 100K-500K rows, not 30K.
- I also realize in hindsight that the entire use case, while having some value, is somewhere between a leading and lagging indicator. From a strategic standpoint, I'd want a LEADING indicator. I would want to know who is going to be a deadbeat credit card holder when they apply for the credit card, NOT after +6 months of spending. Or maybe look at a patient profile of healthy people and predict who is going to die of COVID. Or a neat one would be looking at a data on prisoners to see who is likely to re-offend violently if we let them out.
