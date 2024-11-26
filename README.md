# Water Quality Prediction

L'obiettivo principale è analizzare i dati sulla qualità dell'acqua e sviluppare modelli predittivi per classificare l'acqua come potabile o non potabile.

## Descrizione

La qualità dell'acqua è una risorsa cruciale per la vita, ma spesso le analisi richiedono strumenti complessi. Questo progetto utilizza tecniche di data mining per:
- Analizzare parametri chimico-fisici di grandi dataset.
- Prevedere la potabilità dell'acqua con modelli di classificazione binaria.
- Sfruttare l'analisi dei dati per supportare decisioni informate nella gestione delle risorse idriche.

## Dataset

Il dataset utilizzato è stato scaricato da [Kaggle](https://www.kaggle.com/), contenente oltre un milione di osservazioni con 24 attributi, tra cui:
- pH
- Concentrazioni di metalli (ferro, piombo, zinco)
- Torbidità
- Temperatura dell'acqua
- Conducibilità

L'attributo target indica se l'acqua è potabile (1) o non potabile (0).

## Modelli Utilizzati

Sono stati implementati diversi modelli predittivi per la classificazione:
1. **Classificatori di Base**:
   - Decision Tree
   - K-Nearest Neighbors (KNN)
   - Support Vector Machines (SVM)
   - Naive Bayes
   - Regressione Logistica

2. **Classificatori Ensemble**:
   - Random Forest
   - AdaBoost
   - XGBoost
   - Voting Ensemble (hard e soft)

3. **Reti Neurali**:
   - Multi-Layer Perceptron (MLP)
   - Artificial Neural Network (ANN)

I modelli sono stati valutati con metriche come **accuratezza**, **precisione**, **recall**, **F1-score** e tramite la **curva ROC**.

## Risultati Principali

| Modello              | Accuratezza | Precisione | Recall  | F1-Score |
|----------------------|-------------|------------|---------|----------|
| Decision Tree        | 0.97637     | 0.98155    | 0.97139 | 0.97645  |
| XGBoost              | 0.98590     | 0.99004    | 0.98190 | 0.98595  |
| AdaBoost             | 0.96805     | 0.98935    | 0.94682 | 0.96761  |
| Random Forest        | 0.97869     | 0.98410    | 0.97345 | 0.97875  |
| MLP                  | 0.96084     | 0.97578    | 0.94579 | 0.96055  |
| ANN                  | 0.94978     | 0.96676    | 0.93248 | 0.94931  |

Il miglior modello è **XGBoost**, con un'accuratezza del 98,59% e un recall del 98,19%.
