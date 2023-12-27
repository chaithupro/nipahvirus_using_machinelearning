## <div align="center">NIPAH VIRUS INFECTION PROBABILITY DETECTOR</div>
### Problem:
Cases of Nipah virus infection are a growing concern due to its potential transmission from animals to humans. In affected regions, the situation might escalate, leading to a shortage of diagnostic devices for detecting the Nipah virus.

### Idea:
In such a scenario, prioritizing patients with a higher probability of Nipah virus infection becomes crucial. For instance, if a situation arises where a limited number of diagnostic devices are available for a large number of patients, the individuals with a higher likelihood of infection should be tested first.

### Solution:
To accomplish this, collecting data on various parameters such as age and symptoms of individuals affected by the Nipah virus is essential. Below is a sample dataset, randomly generated for illustrative purposes:

S.No. | Age (in years) | Body temp. (in °F) | Headache | Fever | Vomiting | Cough | Difficulty in breathing | Infected
:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:
|1. | 38 | 99.42 | 1 | 0 | 1 | 0 | 0 | 0 |
|2. | 72 | 104.65 | 1 | 1 | 1 | 2 | 2 | 1 |
...
|10. | 65 | 102.69 | 1 | 1 | 1 | 1 | 1 | 1 |

**_Note:_**
* In the 'Headache,' 'Fever,' 'Vomiting,' and 'Infected' fields:
   0 – No
   1 – Yes
* For 'Cough' and 'Difficulty in breathing':
   0 – Not at all
   1 – Mild
   2 – Severe

The above dataset is just a randomly generated sample. Actual data might encompass information from a broader populace, possibly 50,000 to 60,000 individuals across regions affected by Nipah virus outbreaks.

A machine learning model can be trained on this data, using 'age' and 'symptoms' as features and 'the probability of infection' as the label. When a new patient arrives, providing their age and symptoms will allow the model to estimate the likelihood of Nipah virus infection.

For example, with a patient reporting:
1. Age - 42 years
2. Body temp. - 102.65 °F
3. Headache - 1
4. Fever - 0
5. Vomiting - 1
6. Cough - 1
7. Difficulty in breathing - 0

The machine might output a probability, for instance, 46% (this is just an example, not a real model output).

This system could be presented as user-friendly software where individuals input their symptoms, and the model predicts their likelihood of being infected with the Nipah virus.

### Requirements
To run this system, the following Python libraries are required:
1. scikit-learn (sklearn)
2. numpy
3. pandas
4. django

