## Summary of Research Paper

Jan Niklas van Detten, Pol Schumacher, Sander J. J. Leemans: An Approximate Inductive Miner. ICPM 2023: 129-136

<img width="700" alt="1" src="https://github.com/user-attachments/assets/4ae2f32e-73fb-431c-acd4-0f99a14aa78f" />
<img width="700" alt="2" src="https://github.com/user-attachments/assets/8781359e-e311-4175-83a5-94d0fcdccec4" />
<img width="700" alt="3" src="https://github.com/user-attachments/assets/6bb09169-8642-49ee-9b85-ec6f57b3367f" />

### Data and Results
The data used for testing is the following:
https://data.4tu.nl/datasets/6f35269e-4ce7-4bc4-9abb-b3cea04cad00

Compared to original results in the research paper, the average fitness and precision is lower than achieved results.
The trends in the original results were successfully observed when tested with multiple BPIC datasets.

When filter steps is changed to "4" and "6", the precision rises to 0.93, however average fitness drops even lower, meaning traces align poorly with the model and resulting in over-generalization.
