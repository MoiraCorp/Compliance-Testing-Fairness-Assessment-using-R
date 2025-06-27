 ![MoiraCorp logo](/assets/images/MoiraCorp_Capture.jpg)
# Compliance Testing - Fairness Assessment using R

## Purpose
<p>
The problem is here to test if in a VC firm, the data-driven process of startup dossier discovery and selection is unbiased and compliant with a declared principle of "fairness". Apart from usual financial assessment, the data-driven selection is based on provided descriptions such as: value proposition, customer's pain points and a list of top benefits for customers.
</p>

<p>We propose here to replace the traditional cumbersome manual process of startup sourcing and screening by the use of a Machine Learning (ML) algorithm based on a three steps process:<br>
<ul>
 <li> activity characterisation using a Natural Language Process (NLP) tagging system</li>
 <li> followed by a K-means clustering algorithm capable of classifying the startups by their activity</li>
 <li> and test if the selection/dismissal of their dossier is a "fair" process</li>
</ul><br>

For preprocessing details see: (https://github.com/MoiraCorp/Innovkg-exercise-km/tree/main/step1/preprocess)

<em><strong>IMPORTANT NOTE:</strong></em> This exercise is using the BH Register of Interest database from <em><strong>25 May 2021</strong></em>
</p>

## Method

 > <p><strong>Step1</strong> - Semantic tagging using the LSEG-PermID (Open Calais) service -> (https://github.com/MoiraCorp/Innovkg-exercise-km/tree/main/step1)</p>
 > <p><strong>Step1</strong> - Load data and libraries in R -> (https://github.com/MoiraCorp/Innovkg-exercise-km/tree/main/step1)</p>
 > <p><strong>Step2</strong> - Perform Principal Component Analysis (PCA) and evaluate clustering potential in various factor scores subspaces -> (https://github.com/MoiraCorp/Innovkg-exercise-km/tree/main/step2)</p>
 > <p><strong>Step3</strong> - Perform K-means on a factor scores sub-space at evaluate performance with a minimum number of clusters -> (https://github.com/MoiraCorp/Innovkg-exercise-km/tree/main/step3)</p>
 > <p><strong>Step4</strong> - Display retained clusters statistics -> (https://github.com/MoiraCorp/Innovkg-exercise-km/tree/main/step4)</p>
 > <p><strong>Step5</strong> - Evaluate fairness of Basing Hall-BIC selection process -> (https://github.com/MoiraCorp/Innovkg-exercise-km/tree/main/step5)</p>

