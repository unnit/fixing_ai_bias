# AIF 360 - Bias Mitigation on Financial Dataset
The AI Fairness 360 (AIF360) is an open-source toolkit developed by IBM for detecting and mitigating bias in machine learning models. It is designed to help ensure that AI systems make decisions that are fair and unbiased, as biased systems can result in discrimination, perpetuating inequalities in various domains like healthcare, finance, hiring, and more.
<br/>
One popular in-processing technique is Adversarial Debiasing, which trains a model while simultaneously minimizing bias.
How It Works:
1. Main Model (Predictor): Trains to predict the target variable (Approved column).
2. Adversary (Fairness Critic): Tries to predict the protected attribute (Gender) based on the model's predictions.
3. Loss Adjustment:
- If the adversary can easily predict the protected attribute, it means the main model is using biased information.
- The main model adjusts its learning to make it harder for the adversary, reducing bias.
4. Fairness-Accuracy Tradeoff:
- A higher adversary loss weight reduces bias but may impact accuracy.
- A lower adversary loss weight maintains accuracy but allows some bias.

# Differential Privacy on Facial Recognition

The Laplace mechanism adds random noise drawn from a Laplace distribution to the feature vector.
The amount of noise is controlled by the privacy budget (epsilon) and the sensitivity of the data.
A smaller epsilon value results in more noise and stronger privacy protection.
<br/>
Apply differential privacy on feature vectors which is the privacy preserving technique.The randomise function of the Laplace mechanism is used to add noise to the feature vector, making it differentially private.

# Fixing Bias on a synthentic dataset - Apply Exponentiated Gradient (EG) with Equalized Odds constraints.
The Exponentiated Gradient (EG) method with Equalized Odds constraints has successfully reduced the gender bias by ensuring that the model gives nearly identical treatment to both males and females. The model has become more equitable, with only a slight difference in outcomes for both genders.
