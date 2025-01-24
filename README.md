## Summary of Research Paper

Jan Niklas van Detten, Pol Schumacher, Sander J. J. Leemans: An Approximate Inductive Miner. ICPM 2023: 129-136

<img width="800" alt="1" src="https://github.com/user-attachments/assets/4ae2f32e-73fb-431c-acd4-0f99a14aa78f" />
<img width="800" alt="2" src="https://github.com/user-attachments/assets/8781359e-e311-4175-83a5-94d0fcdccec4" />
<img width="800" alt="3" src="https://github.com/user-attachments/assets/6bb09169-8642-49ee-9b85-ec6f57b3367f" />

### Data and Results for replication
The data used for testing is the following:
https://data.4tu.nl/datasets/6f35269e-4ce7-4bc4-9abb-b3cea04cad00

Compared to original results in the research paper, the average fitness and precision is lower.
When filter steps is changed to "4" and "6", the precision rises to 0.93, however average fitness drops even lower, meaning traces align poorly with the model and resulting in over-generalization.

### Conclusion
The size of the models and the precision difference in the results compared to the original results indicates issues with filtering and clustering (quality estimation).
Over-filtering and under-filtering during event-log preprocessing can lead to information loss.
The clustering and quality estimation can especially be difficult to properly tune:
- Wrong clustering leads to suboptimal quality cuts which do not properly reflect the log’s structure, therefore leading to poor precision.
- Misalignment in operator selection can cause the discovered tree to deviate from the true behavior in the event log.
