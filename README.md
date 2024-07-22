# Team AutoGluon or Off?
As machine learning technology becomes increasingly essential across various industries, there is a growing demand for tools that simplify the development and deployment of ML models. AutoGluon claims to offer a user-friendly platform that requires minimal coding and ML domain knowledge, making it potentially ideal for non-technical users.

This research project aims to evaluate the suitability of AutoGluon, an automated machine learning (AutoML) framework, for non-technical or semi-technical workers seeking to incorporate machine learning (ML) into their professional activities. The study will compare AutoGluon's usability, accessibility, and performance against other well-known ML algorithms such as CatBoost and XGBoost.

The project will specifically assess whether AutoGluon can enable non-technical users to effectively and efficiently apply ML to solve real-world problems, comparing it to the more traditional, yet popular, ML frameworks like CatBoost and XGBoost. The comparison will focus on key metrics such as ease of use, learning curve, model accuracy, and the overall time required from data input to actionable outputs.

By providing clear, empirical data on how well AutoGluon and other algorithms meet the needs of non-technical users, this research will guide organizations and individuals in selecting the most appropriate ML tools for their needs, potentially democratizing the use of machine learning technology.

The notebook used to complete this research can be found here. Below you will find the notebook highlights as well as a summary of findings.

![Notebook Preview](screenshot1.png)
![Notebook Preview](screenshot2.png)
![Notebook Preview](screenshot3.png)

### Model Performance
* XGBoost Default: Achieved an accuracy of 86.37%, which is competitive considering no parameter tuning was applied.
* XGBoost Hypertuned: Slight improvement with tuned parameters, reaching an accuracy of 86.67%. This reflects the benefits of optimizing model parameters.
* AutoGluon: Very close to hypertuned XGBoost with an accuracy of 86.54%, demonstrating strong performance with default settings.

### Explainability
**Model Transparency:**
* XGBoost Models: These are inherently more transparent than many black-box models because they are based on decision trees. Trees can be visualized, and paths can be traced, which makes them relatively understandable.
* AutoGluon: Depending on which model or ensemble of models AutoGluon chooses, the transparency can vary. If AutoGluon selects tree-based models, the explainability might be similar to XGBoost. However, if it selects other model types like neural networks, explainability might decrease.

**Tools:**
* Both XGBoost and tree-based models in AutoGluon can be analyzed using SHAP (SHapley Additive exPlanations), which provides a powerful framework for understanding feature contributions to model outputs.
* The assumption here is that these tools accurately reflect the contribution of each feature to the decision-making process, which relies on the mathematical soundness of SHAP and its implementation.

### Practicality
**Learning Curve:** XGBoost requires a gradual learning curve, with more depth needed for tuning. AutoGluon offers a less steep initial learning curve due to its simplicity and automation, making it ideal for those who want effective results without deep diving into ML mechanics.
* Hypertuning XGBoost requires more effort and understanding of the model’s parameters and a good grasp of how tuning affects model performance, overfitting, and underfitting.
* Significant time is needed not only to run the hypertuning process, but also explain the results. Resources (financial and computational) are also needed.

**Application in Daily Tasks:** For a financial analyst at a tech company, using AutoGluon may allow more time to focus on data interpretation and decision-making rather than on model training and optimization.

**Long-Term Skill Development:** Learning to use XGBoost effectively, including its hypertuning, can be more beneficial for career growth in data science due to the widespread use and respect for the versatility of the XGBoost algorithm in the industry.
