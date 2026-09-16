# Topics learned:-
types of ml ny how the model learns over times (batch /online learning )

# Key concepts:-
Batch ML vs Online ML

The main difference is how the model learns from new data.

Feature	Batch ML	Online ML
Training	Trains on a large dataset at once	Learns continuously from incoming data
Data	Usually static/historical	Continuously arriving
Updates	Periodic retraining	Frequent/continuous updates
Speed	Training can be slow	Each update is usually fast
Memory	Can require lots of storage/RAM	Can work with small amounts of data
Best for	Stable datasets	Changing/streaming data
Example	House-price prediction	Fraud detection
🟦 Batch Machine Learning

Suppose you have 10 million historical house records.

You:

10 million records
       ↓
Train model
       ↓
Model v1
       ↓
Deploy

When you get new data, the model doesn't automatically learn from it.

You might retrain every week/month:

New data
   ↓
Add to dataset
   ↓
Retrain model
   ↓
New model

Example: Predicting house prices where the underlying patterns don't change extremely quickly.

🟩 Online Machine Learning

The model learns incrementally as new data arrives.

Data 1 → Model updates
Data 2 → Model updates
Data 3 → Model updates
Data 4 → Model updates
       ↓
Continuously improving model

For example, imagine a spam detector:

Email → Model → Spam
              ↓
        User says "Not spam"
              ↓
        Model learns from it

This is useful when the data distribution changes over time (concept drift).

Easy way to remember

Batch ML = Learn in chunks
Online ML = Learn continuously

# Tomorrow
types of ml on how the model generalizes.