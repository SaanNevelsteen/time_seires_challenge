##

Baseline experiment:

wordt uitgevoerd in Full mode (11138 spectogrammen en 88 features)
model: Histogram Gradient Boosting (>= 10 stemmen)
    - Prior KL: 1.2071
    - Logistic Regression KL: 1.1048
    - HGB KL: 0.9046 

model: Histogram Gradient Boosting (all EEG's)
    - Prior KL: 1.2559
    - Logistic Regression KL: 1.1136
    - HGB KL: 0.9343

gameplan:
2 experimenten uitvoeren 
    1)
    - extra kenmerken toevoegen uit 20 seconden EEG
    - doel: betere informatie voor het model
    2)
    - ander machinelearningalgoritme
    - doel: betere voorspellingen met dezelfde informatie


experiment 1)
- ik heb 16 extra kenmekren toegevoegd, deze bereken het gemiddelde logaritmische vermogen per hersenregio en frequentieband in een centraal venster van 20 seconden
- model: Histrogram Gradient boosting
- KL op alle EEG's: 0.8651
- KL op >= 10 stemmen: 0.8334
- dit suggereert dat kortdurende informatie nuttig is voor classificatie 
 