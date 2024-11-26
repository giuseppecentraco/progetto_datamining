# Water Quality Prediction

L'obiettivo principale è analizzare i dati sulla qualità dell'acqua e sviluppare modelli predittivi per classificare l'acqua come potabile o non potabile.

## Descrizione

La qualità dell'acqua è una risorsa cruciale per la vita, ma spesso le analisi richiedono strumenti complessi. Questo progetto utilizza tecniche di data mining per:
- Analizzare parametri chimico-fisici di grandi dataset.
- Prevedere la potabilità dell'acqua con modelli di classificazione binaria.
- Sfruttare l'analisi dei dati per supportare decisioni informate nella gestione delle risorse idriche.

## Contenuto del Repository

- **`WaterQualityPrediction-Centraco.ipynb`**: Il notebook Jupyter contiene l'intero progetto, inclusi i passi di preprocessing, l'analisi esplorativa dei dati (EDA), la costruzione e la valutazione dei modelli predittivi.
- **`Presentazione WaterQualityPrediction.pdf`**: File PDF che offre una panoramica completa del progetto, descrivendo i principali risultati e le metodologie utilizzate.
- **`README.md`**: Documentazione del progetto (questo file).

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

| Modello                      | Accuratezza | Precisione | Recall  | F1-Score |
|------------------------------|-------------|------------|---------|----------|
| Albero Decisionale           | 0.97637     | 0.98155    | 0.97139 | 0.97645  |
| Albero Decisionale GSCV      | 0.97386     | 0.97725    | 0.97076 | 0.97399  |
| KNN                          | 0.88135     | 0.98938    | 0.77296 | 0.86788  |
| KNN GSCV                     | 0.89562     | 0.97555    | 0.81334 | 0.88709  |
| SVM                          | 0.95514     | 0.98476    | 0.92422 | 0.95353  |
| Naive Bayes                  | 0.81586     | 0.98667    | 0.64343 | 0.77892  |
| Naive Bayes GSCV             | 0.81590     | 0.98679    | 0.64343 | 0.77895  |
| Regressione Logistica        | 0.86833     | 0.90211    | 0.82875 | 0.86387  |
| Regressione Logistica GSCV   | 0.86805     | 0.90108    | 0.82930 | 0.86370  |
| SGD                          | 0.86681     | 0.89658    | 0.83175 | 0.86295  |
| SGD GSCV                     | 0.86530     | 0.89850    | 0.82614 | 0.86080  |
| Random Forest                | 0.97869     | 0.98410    | 0.97345 | 0.97875  |
| AdaBoost                     | 0.96805     | 0.98935    | 0.94682 | 0.96761  |
| XGBoost                      | 0.98590     | 0.99004    | 0.98190 | 0.98595  |
| Voting Hard                  | 0.90793     | 0.99117    | 0.82472 | 0.90031  |
| Voting Soft                  | 0.94645     | 0.98792    | 0.90485 | 0.94456  |
| MLP                          | 0.96084     | 0.97578    | 0.94579 | 0.96055  |
| ANN                          | 0.94978     | 0.96676    | 0.93248 | 0.94931  |

Il miglior modello è **XGBoost**, con un'accuratezza del 98,59% e un recall del 98,19%.
