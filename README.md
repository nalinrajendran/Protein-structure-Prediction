# Protein-structure-Prediction
This Is a Q Learning model, which predicts the structure of the given protein Input.


The following AI project uses reinforcement learning to attempt to resolve a condensed form of the Protein Structure Prediction (PSP) problem. Finding the native state of a protein given its amino acid sequence is the focus of the protein structure prediction problem. When a protein is synthesized, it folds rapidly in the space until it reaches a stable form, usually referred to as the Native State. The protein can then perform its designated job after that. 

One of the biggest issues in bioinformatics is predicting the outcome of the folding process in advance. Solving this problem would have significant ramifications for many fields, from biochemistry to genetic engineering.



Create a virtual environment first

>> conda create --name pspenv
>> conda activate pspenv

Installing the pre-Requisites
>> cd path/to/Protein-Structure-Prediction
>> pip install -r requirements.txt

>>python3 setup.py install

Running the Model

>> psp-cli train q models/q_agent.pkl --seq HHPPHH
By default, the model trains upto 50000 episodes(5 iterations), you can modify it by adding --episodes 60000 or anynumber of your wish.

>> psp-cli run q models/q_agent.pkl --seq HPHPH


For more options

>>psp-cli -h


It displays all the options availabe over there.
