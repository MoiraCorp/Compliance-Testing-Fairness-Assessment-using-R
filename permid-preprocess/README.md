# Preprocessing: Extracting activity semantic tags using LSEG PermID Intelligent Tagging (Open Calais)

## What is LSEG-PermID?

<p> LSEG is providing several services aiming at providing Permanent Identifiers (PermIDs) for tagging financial related information related to any product or company. These services are regrouped under the PermID "banner" ( https://permid.org/ ). These services are delivered in "Open" mode. They are intended to facilitate and standardize the information exchanged between the various stakeholders of the economics sector. This service inherits from an older product named "Open Calais" which was acquired from Reuters about 10 years ago ( https://en.wikipedia.org/wiki/Calais_(Reuters_product) )</p> 

<p>This technology was originally developed by a US-Israel company named ClearForest which was later acquired by Reuters. The provided on-line service and its dictionary and data structures are built around a concept known as the "Semantic Web" ( https://en.wikipedia.org/wiki/Semantic_Web ). This technology and its standards were introduced in 2001 by Berners-Lee and his colleagues as a way of describing on the Web the relations between the "meaning" of published data or information.</p>

## What is the semantic tagging service offered by PermID?

<p>In its present PermID version, the "Open Calais" engine extracts semantic information from any provided text in .txt, .pdf, .xml or .html format. It uses advanced natural language processing technologies in order to confront the submitted text with a huge semantic database and returns a list of the most significant keywords found to relate to the submitted document. These keywords are organized in several sets: Category, Industry, Social Tags and Individuals.</p>

## Using PermID "Intelligent Tagging" on the VC "Statement of Interest" Questionnaire

<p>The preprocessing phase uses the Register of Interest database generated from the on-line questionnaire submitted to each startup<br>
For each company in the database, semantic tags identified using the LSEG-PermID Intelligent Tagging (Open Calais) service from the juxtaposition of 3 descriptive fields present in the database.<br> These fields are respectively:<br> 
<ul>
  <li>2.2 Value Proposition</li>
  <li>2.3 Customer's pain points</li>
  <li>2.4 TOP benefits for customer</li>
</ul><br>

The activity "tags" determined by PermID from the concatenation of these 3 questionnaire fields are:
<ul>
<li>A1 - Religion_Belief</li>
<li>A2 - War_Conflict</li>
<li>A3 - Business_Finance</li>
<li>A4 - Health_Medical_Pharma</li>
<li>A5 - Labor</li>
<li>A6 - Entertainment_Culture</li>
<li>A7 - Social Issues</li>
<li>A8 - Education</li>
<li>A9 - Technology_Internet</li>
<li>A10 - Environment_Agriculture</li>
<li>A11 - Human Interest</li>
<li>A12 - Hospitality_Recreation</li>
<li>A13 - Disaster_Accident</li>
<li>A14 - Politics</li>
<li>A15 - Sports</li>
<li>A16 - Law_Crime</li>
</ul>

## The final PermID encoded Questionnaire

<p>For the 529 startup companies registered in the questionnaire, the final PermID encoded questionnaire is presented in table: BH_OCC_wStatus-IDSorted_24-Mar-2021.csv ( https://github.com/MoiraCorp/Compliance-Testing-Fairness-Assessment-using-R/blob/main/permid-preprocess/BH_OCC_wStatus-IDSorted_24-Mar-2021.csv )</p>

Regarding this datatable it is important to note:
> Each of the semantic tags A1 to A16 is represented by a probability of being associated with the descriptive text submitted by each startup<br>
> The "Status" column provides a list of actions taken by the VC firm staff regarding a particular startup submission dossier<br>

The possible "Status" codes are:
<ul>
<li>1. Form Submitted</li>
<li>2. Initial Contact Phase</li>
<li>3. First interview</li>
<li>4. Deal call candidate</li>
<li>5. Deal Call Pre-selection</li>
<li>6. Q&A</li>
<li>7. Deal call TOP 10</li>
<li>8. Deal call TOP 5</li>
<li>9. BAQ</li>
<li>16. Closed</li>
<li>19. BAQ not returned</li>
<li>20. Further to follow</li>
<li>21. Discontinued</li>
<li>22. Dismissed</li>
</ul>
