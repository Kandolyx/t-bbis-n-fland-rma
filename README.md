
![image](https://github.com/user-attachments/assets/d5f888ae-5de5-4e3c-8fbe-8a9088b6984d)

![image](https://github.com/user-attachments/assets/e43dedde-0a17-4e9c-abbc-1f07bfcade97)

![image](https://github.com/user-attachments/assets/5f4a25e6-d739-42b5-bc89-1e9193517680)

![image](https://github.com/user-attachments/assets/2f203f32-0091-4e11-8058-f010e55e74cd)

![image](https://github.com/user-attachments/assets/c96e6f0f-c62e-4866-ae26-5a4d7bb87dd4)


![image](https://github.com/user-attachments/assets/a0b8395b-dd38-49da-b81f-0939aa04ef89)






⚙️ Özellik Seti: TF-IDF


🎯 XGBoost eğitiliyor... (SMOTE: Hayır)
/usr/local/lib/python3.11/dist-packages/xgboost/training.py:183: UserWarning: [18:33:23] WARNING: /workspace/src/learner.cc:738: 
Parameters: { "predictor", "use_label_encoder" } are not used.

  bst.update(dtrain, iteration=i, fobj=obj)
⏱️ Eğitim Süresi: 40.73 saniye
              precision    recall  f1-score   support

           1       0.66      0.64      0.65       633
           2       0.38      0.35      0.36       299
           3       0.37      0.26      0.31       385
           4       0.60      0.56      0.58       610
           5       0.38      0.45      0.41       961

    accuracy                           0.48      2888
   macro avg       0.48      0.45      0.46      2888
weighted avg       0.49      0.48      0.48      2888


🎯 Linear SVM eğitiliyor... (SMOTE: Hayır)
⏱️ Eğitim Süresi: 1.77 saniye
              precision    recall  f1-score   support

           1       0.71      0.76      0.74       633
           2       0.55      0.48      0.51       299
           3       0.53      0.42      0.47       385
           4       0.67      0.69      0.68       610
           5       0.51      0.54      0.53       961

    accuracy                           0.60      2888
   macro avg       0.59      0.58      0.58      2888
weighted avg       0.59      0.60      0.59      2888


🎯 LogisticRegression eğitiliyor... (SMOTE: Hayır)
/usr/local/lib/python3.11/dist-packages/sklearn/linear_model/_logistic.py:465: ConvergenceWarning: lbfgs failed to converge (status=1):
STOP: TOTAL NO. OF ITERATIONS REACHED LIMIT.

Increase the number of iterations (max_iter) or scale the data as shown in:
    https://scikit-learn.org/stable/modules/preprocessing.html
Please also refer to the documentation for alternative solver options:
    https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression
  n_iter_i = _check_optimize_result(
/usr/local/lib/python3.11/dist-packages/sklearn/metrics/_classification.py:1565: UndefinedMetricWarning: Precision is ill-defined and being set to 0.0 in labels with no predicted samples. Use `zero_division` parameter to control this behavior.
  _warn_prf(average, modifier, f"{metric.capitalize()} is", len(result))
/usr/local/lib/python3.11/dist-packages/sklearn/metrics/_classification.py:1565: UndefinedMetricWarning: Precision is ill-defined and being set to 0.0 in labels with no predicted samples. Use `zero_division` parameter to control this behavior.
  _warn_prf(average, modifier, f"{metric.capitalize()} is", len(result))
/usr/local/lib/python3.11/dist-packages/sklearn/metrics/_classification.py:1565: UndefinedMetricWarning: Precision is ill-defined and being set to 0.0 in labels with no predicted samples. Use `zero_division` parameter to control this behavior.
  _warn_prf(average, modifier, f"{metric.capitalize()} is", len(result))
⏱️ Eğitim Süresi: 9.30 saniye
              precision    recall  f1-score   support

           1       0.83      0.19      0.31       633
           2       0.00      0.00      0.00       299
           3       0.00      0.00      0.00       385
           4       0.41      0.36      0.38       610
           5       0.35      0.82      0.49       961

    accuracy                           0.39      2888
   macro avg       0.32      0.27      0.24      2888
weighted avg       0.39      0.39      0.31      2888


🎯 RandomForest eğitiliyor... (SMOTE: Hayır)
⏱️ Eğitim Süresi: 92.05 saniye
              precision    recall  f1-score   support

           1       0.66      0.65      0.66       633
           2       0.34      0.30      0.32       299
           3       0.34      0.22      0.27       385
           4       0.57      0.61      0.59       610
           5       0.36      0.41      0.39       961

    accuracy                           0.47      2888
   macro avg       0.45      0.44      0.44      2888
weighted avg       0.47      0.47      0.47      2888


🎯 LightGBM eğitiliyor... (SMOTE: Hayır)
[LightGBM] [Info] Auto-choosing col-wise multi-threading, the overhead of testing was 0.057335 seconds.
You can set `force_col_wise=true` to remove the overhead.
[LightGBM] [Info] Total Bins 143376
[LightGBM] [Info] Number of data points in the train set: 11550, number of used features: 1002
[LightGBM] [Info] Start training from score -1.518466
[LightGBM] [Info] Start training from score -2.268539
[LightGBM] [Info] Start training from score -2.014903
[LightGBM] [Info] Start training from score -1.554278
[LightGBM] [Info] Start training from score -1.100172
/usr/local/lib/python3.11/dist-packages/sklearn/utils/validation.py:2739: UserWarning: X does not have valid feature names, but LGBMClassifier was fitted with feature names
  warnings.warn(
⏱️ Eğitim Süresi: 13.95 saniye
              precision    recall  f1-score   support

           1       0.67      0.68      0.68       633
           2       0.38      0.39      0.39       299
           3       0.40      0.31      0.35       385
           4       0.60      0.60      0.60       610
           5       0.40      0.42      0.41       961

    accuracy                           0.50      2888
   macro avg       0.49      0.48      0.48      2888
weighted avg       0.50      0.50      0.50      2888

🔁 SMOTE uygulanıyor...


🎯 XGBoost eğitiliyor... (SMOTE: Evet)
/usr/local/lib/python3.11/dist-packages/xgboost/training.py:183: UserWarning: [18:36:03] WARNING: /workspace/src/learner.cc:738: 
Parameters: { "predictor", "use_label_encoder" } are not used.

  bst.update(dtrain, iteration=i, fobj=obj)
⏱️ Eğitim Süresi: 53.41 saniye
              precision    recall  f1-score   support

           1       0.68      0.67      0.67       633
           2       0.40      0.39      0.39       299
           3       0.42      0.36      0.38       385
           4       0.61      0.59      0.60       610
           5       0.38      0.42      0.40       961

    accuracy                           0.50      2888
   macro avg       0.50      0.48      0.49      2888
weighted avg       0.50      0.50      0.50      2888


🎯 Linear SVM eğitiliyor... (SMOTE: Evet)
⏱️ Eğitim Süresi: 3.41 saniye
              precision    recall  f1-score   support

           1       0.68      0.81      0.74       633
           2       0.43      0.74      0.54       299
           3       0.41      0.72      0.52       385
           4       0.64      0.80      0.71       610
           5       0.66      0.13      0.22       961

    accuracy                           0.56      2888
   macro avg       0.56      0.64      0.55      2888
weighted avg       0.60      0.56      0.51      2888


🎯 LogisticRegression eğitiliyor... (SMOTE: Evet)
/usr/local/lib/python3.11/dist-packages/sklearn/linear_model/_logistic.py:465: ConvergenceWarning: lbfgs failed to converge (status=1):
STOP: TOTAL NO. OF ITERATIONS REACHED LIMIT.

Increase the number of iterations (max_iter) or scale the data as shown in:
    https://scikit-learn.org/stable/modules/preprocessing.html
Please also refer to the documentation for alternative solver options:
    https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression
  n_iter_i = _check_optimize_result(
⏱️ Eğitim Süresi: 18.67 saniye
              precision    recall  f1-score   support

           1       0.68      0.63      0.65       633
           2       0.40      0.50      0.44       299
           3       0.24      0.62      0.35       385
           4       0.50      0.46      0.48       610
           5       0.44      0.17      0.24       961

    accuracy                           0.43      2888
   macro avg       0.45      0.48      0.43      2888
weighted avg       0.47      0.43      0.42      2888


🎯 RandomForest eğitiliyor... (SMOTE: Evet)
⏱️ Eğitim Süresi: 266.37 saniye
              precision    recall  f1-score   support

           1       0.66      0.64      0.65       633
           2       0.36      0.42      0.39       299
           3       0.38      0.36      0.37       385
           4       0.57      0.60      0.58       610
           5       0.37      0.35      0.36       961

    accuracy                           0.47      2888
   macro avg       0.47      0.47      0.47      2888
weighted avg       0.47      0.47      0.47      2888


🎯 LightGBM eğitiliyor... (SMOTE: Evet)
[LightGBM] [Info] Auto-choosing col-wise multi-threading, the overhead of testing was 0.166846 seconds.
You can set `force_col_wise=true` to remove the overhead.
[LightGBM] [Info] Total Bins 221105
[LightGBM] [Info] Number of data points in the train set: 19220, number of used features: 1002
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
/usr/local/lib/python3.11/dist-packages/sklearn/utils/validation.py:2739: UserWarning: X does not have valid feature names, but LGBMClassifier was fitted with feature names
  warnings.warn(
⏱️ Eğitim Süresi: 24.15 saniye
              precision    recall  f1-score   support

           1       0.69      0.69      0.69       633
           2       0.40      0.44      0.42       299
           3       0.42      0.39      0.41       385
           4       0.61      0.63      0.62       610
           5       0.42      0.41      0.41       961

    accuracy                           0.52      2888
   macro avg       0.51      0.51      0.51      2888
weighted avg       0.52      0.52      0.52      2888


⚙️ Özellik Seti: BERT
/usr/local/lib/python3.11/dist-packages/huggingface_hub/utils/_auth.py:94: UserWarning: 
The secret `HF_TOKEN` does not exist in your Colab secrets.
To authenticate with the Hugging Face Hub, create a token in your settings tab (https://huggingface.co/settings/tokens), set it as secret in your Google Colab and restart your session.
You will be able to reuse this secret in all of your notebooks.
Please note that authentication is recommended but still optional to access public models or datasets.
  warnings.warn(
BERT Batch İşleniyor: 100%|██████████| 452/452 [00:24<00:00, 18.72it/s]
💾 Embedding'ler kaydedildi: bert_only.npy


🎯 XGBoost eğitiliyor... (SMOTE: Hayır)
/usr/local/lib/python3.11/dist-packages/xgboost/training.py:183: UserWarning: [18:42:52] WARNING: /workspace/src/learner.cc:738: 
Parameters: { "predictor", "use_label_encoder" } are not used.

  bst.update(dtrain, iteration=i, fobj=obj)
⏱️ Eğitim Süresi: 7.31 saniye
              precision    recall  f1-score   support

           1       0.52      0.50      0.51       633
           2       0.15      0.12      0.13       299
           3       0.24      0.15      0.19       385
           4       0.47      0.43      0.45       610
           5       0.30      0.39      0.34       961

    accuracy                           0.36      2888
   macro avg       0.34      0.32      0.32      2888
weighted avg       0.36      0.36      0.36      2888


🎯 Linear SVM eğitiliyor... (SMOTE: Hayır)
⏱️ Eğitim Süresi: 4.64 saniye
              precision    recall  f1-score   support

           1       0.61      0.69      0.65       633
           2       0.33      0.10      0.16       299
           3       0.45      0.23      0.30       385
           4       0.55      0.59      0.57       610
           5       0.44      0.57      0.50       961

    accuracy                           0.51      2888
   macro avg       0.48      0.44      0.44      2888
weighted avg       0.49      0.51      0.48      2888


🎯 LogisticRegression eğitiliyor... (SMOTE: Hayır)
/usr/local/lib/python3.11/dist-packages/sklearn/linear_model/_logistic.py:465: ConvergenceWarning: lbfgs failed to converge (status=1):
STOP: TOTAL NO. OF ITERATIONS REACHED LIMIT.

Increase the number of iterations (max_iter) or scale the data as shown in:
    https://scikit-learn.org/stable/modules/preprocessing.html
Please also refer to the documentation for alternative solver options:
    https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression
  n_iter_i = _check_optimize_result(
⏱️ Eğitim Süresi: 77.28 saniye
              precision    recall  f1-score   support

           1       0.57      0.63      0.60       633
           2       0.22      0.08      0.11       299
           3       0.49      0.21      0.29       385
           4       0.57      0.50      0.53       610
           5       0.41      0.58      0.48       961

    accuracy                           0.47      2888
   macro avg       0.45      0.40      0.40      2888
weighted avg       0.47      0.47      0.45      2888


🎯 RandomForest eğitiliyor... (SMOTE: Hayır)
⏱️ Eğitim Süresi: 17.47 saniye
              precision    recall  f1-score   support

           1       0.51      0.49      0.50       633
           2       0.04      0.02      0.03       299
           3       0.15      0.07      0.09       385
           4       0.45      0.39      0.42       610
           5       0.29      0.43      0.34       961

    accuracy                           0.34      2888
   macro avg       0.29      0.28      0.28      2888
weighted avg       0.33      0.34      0.33      2888


🎯 LightGBM eğitiliyor... (SMOTE: Hayır)
[LightGBM] [Info] Auto-choosing col-wise multi-threading, the overhead of testing was 0.008323 seconds.
You can set `force_col_wise=true` to remove the overhead.
[LightGBM] [Info] Total Bins 33150
[LightGBM] [Info] Number of data points in the train set: 11550, number of used features: 130
[LightGBM] [Info] Start training from score -1.518466
[LightGBM] [Info] Start training from score -2.268539
[LightGBM] [Info] Start training from score -2.014903
[LightGBM] [Info] Start training from score -1.554278
[LightGBM] [Info] Start training from score -1.100172
/usr/local/lib/python3.11/dist-packages/sklearn/utils/validation.py:2739: UserWarning: X does not have valid feature names, but LGBMClassifier was fitted with feature names
  warnings.warn(
⏱️ Eğitim Süresi: 3.90 saniye
              precision    recall  f1-score   support

           1       0.55      0.55      0.55       633
           2       0.17      0.11      0.13       299
           3       0.25      0.15      0.19       385
           4       0.49      0.46      0.47       610
           5       0.31      0.40      0.35       961

    accuracy                           0.39      2888
   macro avg       0.35      0.34      0.34      2888
weighted avg       0.38      0.39      0.38      2888

🔁 SMOTE uygulanıyor...


🎯 XGBoost eğitiliyor... (SMOTE: Evet)
/usr/local/lib/python3.11/dist-packages/xgboost/training.py:183: UserWarning: [18:44:44] WARNING: /workspace/src/learner.cc:738: 
Parameters: { "predictor", "use_label_encoder" } are not used.

  bst.update(dtrain, iteration=i, fobj=obj)
⏱️ Eğitim Süresi: 9.03 saniye
              precision    recall  f1-score   support

           1       0.55      0.53      0.54       633
           2       0.20      0.23      0.22       299
           3       0.26      0.25      0.25       385
           4       0.46      0.45      0.45       610
           5       0.30      0.30      0.30       961

    accuracy                           0.37      2888
   macro avg       0.35      0.35      0.35      2888
weighted avg       0.37      0.37      0.37      2888


🎯 Linear SVM eğitiliyor... (SMOTE: Evet)
⏱️ Eğitim Süresi: 6.35 saniye
              precision    recall  f1-score   support

           1       0.61      0.67      0.64       633
           2       0.27      0.58      0.37       299
           3       0.35      0.53      0.42       385
           4       0.54      0.67      0.60       610
           5       0.51      0.11      0.18       961

    accuracy                           0.46      2888
   macro avg       0.46      0.51      0.44      2888
weighted avg       0.49      0.46      0.42      2888


🎯 LogisticRegression eğitiliyor... (SMOTE: Evet)
/usr/local/lib/python3.11/dist-packages/sklearn/linear_model/_logistic.py:465: ConvergenceWarning: lbfgs failed to converge (status=1):
STOP: TOTAL NO. OF ITERATIONS REACHED LIMIT.

Increase the number of iterations (max_iter) or scale the data as shown in:
    https://scikit-learn.org/stable/modules/preprocessing.html
Please also refer to the documentation for alternative solver options:
    https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression
  n_iter_i = _check_optimize_result(
⏱️ Eğitim Süresi: 78.09 saniye
              precision    recall  f1-score   support

           1       0.59      0.62      0.60       633
           2       0.25      0.52      0.34       299
           3       0.33      0.48      0.39       385
           4       0.54      0.60      0.57       610
           5       0.43      0.16      0.23       961

    accuracy                           0.43      2888
   macro avg       0.43      0.47      0.43      2888
weighted avg       0.45      0.43      0.42      2888


🎯 RandomForest eğitiliyor... (SMOTE: Evet)
⏱️ Eğitim Süresi: 31.34 saniye
              precision    recall  f1-score   support

           1       0.51      0.54      0.52       633
           2       0.17      0.24      0.20       299
           3       0.26      0.29      0.27       385
           4       0.44      0.48      0.46       610
           5       0.20      0.14      0.17       961

    accuracy                           0.33      2888
   macro avg       0.31      0.34      0.32      2888
weighted avg       0.32      0.33      0.32      2888


🎯 LightGBM eğitiliyor... (SMOTE: Evet)
[LightGBM] [Info] Auto-choosing col-wise multi-threading, the overhead of testing was 0.017197 seconds.
You can set `force_col_wise=true` to remove the overhead.
[LightGBM] [Info] Total Bins 33150
[LightGBM] [Info] Number of data points in the train set: 19220, number of used features: 130
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
/usr/local/lib/python3.11/dist-packages/sklearn/utils/validation.py:2739: UserWarning: X does not have valid feature names, but LGBMClassifier was fitted with feature names
  warnings.warn(
⏱️ Eğitim Süresi: 4.88 saniye
              precision    recall  f1-score   support

           1       0.57      0.58      0.58       633
           2       0.21      0.25      0.23       299
           3       0.29      0.27      0.28       385
           4       0.49      0.50      0.50       610
           5       0.31      0.29      0.30       961

    accuracy                           0.39      2888
   macro avg       0.37      0.38      0.38      2888
weighted avg       0.39      0.39      0.39      2888


⚙️ Özellik Seti: BERT + TF-IDF
BERT Batch İşleniyor: 100%|██████████| 452/452 [00:21<00:00, 20.64it/s]
💾 Embedding'ler kaydedildi: bert_tfidf.npy


🎯 XGBoost eğitiliyor... (SMOTE: Hayır)
/usr/local/lib/python3.11/dist-packages/xgboost/training.py:183: UserWarning: [18:47:21] WARNING: /workspace/src/learner.cc:738: 
Parameters: { "predictor", "use_label_encoder" } are not used.

  bst.update(dtrain, iteration=i, fobj=obj)
⏱️ Eğitim Süresi: 50.28 saniye
              precision    recall  f1-score   support

           1       0.64      0.62      0.63       633
           2       0.35      0.30      0.33       299
           3       0.36      0.27      0.31       385
           4       0.59      0.57      0.58       610
           5       0.36      0.43      0.40       961

    accuracy                           0.47      2888
   macro avg       0.46      0.44      0.45      2888
weighted avg       0.47      0.47      0.47      2888


🎯 Linear SVM eğitiliyor... (SMOTE: Hayır)
⏱️ Eğitim Süresi: 15.98 saniye
              precision    recall  f1-score   support

           1       0.70      0.74      0.72       633
           2       0.51      0.45      0.48       299
           3       0.56      0.42      0.48       385
           4       0.66      0.69      0.67       610
           5       0.50      0.54      0.52       961

    accuracy                           0.59      2888
   macro avg       0.59      0.57      0.57      2888
weighted avg       0.59      0.59      0.59      2888


🎯 LogisticRegression eğitiliyor... (SMOTE: Hayır)
/usr/local/lib/python3.11/dist-packages/sklearn/linear_model/_logistic.py:465: ConvergenceWarning: lbfgs failed to converge (status=1):
STOP: TOTAL NO. OF ITERATIONS REACHED LIMIT.

Increase the number of iterations (max_iter) or scale the data as shown in:
    https://scikit-learn.org/stable/modules/preprocessing.html
Please also refer to the documentation for alternative solver options:
    https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression
  n_iter_i = _check_optimize_result(
⏱️ Eğitim Süresi: 22.62 saniye
              precision    recall  f1-score   support

           1       0.57      0.64      0.60       633
           2       0.23      0.07      0.11       299
           3       0.45      0.25      0.33       385
           4       0.55      0.51      0.53       610
           5       0.40      0.55      0.46       961

    accuracy                           0.47      2888
   macro avg       0.44      0.40      0.41      2888
weighted avg       0.46      0.47      0.45      2888


🎯 RandomForest eğitiliyor... (SMOTE: Hayır)
⏱️ Eğitim Süresi: 209.38 saniye
              precision    recall  f1-score   support

           1       0.63      0.60      0.62       633
           2       0.09      0.05      0.07       299
           3       0.22      0.11      0.14       385
           4       0.56      0.56      0.56       610
           5       0.34      0.47      0.39       961

    accuracy                           0.42      2888
   macro avg       0.37      0.36      0.36      2888
weighted avg       0.41      0.42      0.41      2888


🎯 LightGBM eğitiliyor... (SMOTE: Hayır)
[LightGBM] [Info] Auto-choosing col-wise multi-threading, the overhead of testing was 0.062016 seconds.
You can set `force_col_wise=true` to remove the overhead.
[LightGBM] [Info] Total Bins 176016
[LightGBM] [Info] Number of data points in the train set: 11550, number of used features: 1130
[LightGBM] [Info] Start training from score -1.518466
[LightGBM] [Info] Start training from score -2.268539
[LightGBM] [Info] Start training from score -2.014903
[LightGBM] [Info] Start training from score -1.554278
[LightGBM] [Info] Start training from score -1.100172
/usr/local/lib/python3.11/dist-packages/sklearn/utils/validation.py:2739: UserWarning: X does not have valid feature names, but LGBMClassifier was fitted with feature names
  warnings.warn(
⏱️ Eğitim Süresi: 19.00 saniye
              precision    recall  f1-score   support

           1       0.66      0.66      0.66       633
           2       0.35      0.33      0.34       299
           3       0.37      0.29      0.33       385
           4       0.59      0.58      0.59       610
           5       0.38      0.42      0.40       961

    accuracy                           0.48      2888
   macro avg       0.47      0.46      0.46      2888
weighted avg       0.48      0.48      0.48      2888

🔁 SMOTE uygulanıyor...


🎯 XGBoost eğitiliyor... (SMOTE: Evet)
/usr/local/lib/python3.11/dist-packages/xgboost/training.py:183: UserWarning: [18:52:44] WARNING: /workspace/src/learner.cc:738: 
Parameters: { "predictor", "use_label_encoder" } are not used.

  bst.update(dtrain, iteration=i, fobj=obj)
⏱️ Eğitim Süresi: 63.09 saniye
              precision    recall  f1-score   support

           1       0.66      0.63      0.64       633
           2       0.38      0.38      0.38       299
           3       0.38      0.32      0.35       385
           4       0.59      0.58      0.59       610
           5       0.37      0.41      0.39       961

    accuracy                           0.48      2888
   macro avg       0.48      0.46      0.47      2888
weighted avg       0.48      0.48      0.48      2888


🎯 Linear SVM eğitiliyor... (SMOTE: Evet)
⏱️ Eğitim Süresi: 22.64 saniye
              precision    recall  f1-score   support

           1       0.71      0.76      0.73       633
           2       0.45      0.70      0.54       299
           3       0.45      0.63      0.52       385
           4       0.64      0.74      0.69       610
           5       0.58      0.30      0.40       961

    accuracy                           0.58      2888
   macro avg       0.57      0.63      0.58      2888
weighted avg       0.59      0.58      0.56      2888


🎯 LogisticRegression eğitiliyor... (SMOTE: Evet)
/usr/local/lib/python3.11/dist-packages/sklearn/linear_model/_logistic.py:465: ConvergenceWarning: lbfgs failed to converge (status=1):
STOP: TOTAL NO. OF ITERATIONS REACHED LIMIT.

Increase the number of iterations (max_iter) or scale the data as shown in:
    https://scikit-learn.org/stable/modules/preprocessing.html
Please also refer to the documentation for alternative solver options:
    https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression
  n_iter_i = _check_optimize_result(
⏱️ Eğitim Süresi: 39.06 saniye
              precision    recall  f1-score   support

           1       0.58      0.60      0.59       633
           2       0.25      0.48      0.33       299
           3       0.33      0.50      0.40       385
           4       0.51      0.64      0.57       610
           5       0.45      0.15      0.23       961

    accuracy                           0.43      2888
   macro avg       0.43      0.47      0.42      2888
weighted avg       0.46      0.43      0.41      2888


🎯 RandomForest eğitiliyor... (SMOTE: Evet)
⏱️ Eğitim Süresi: 511.18 saniye
              precision    recall  f1-score   support

           1       0.64      0.63      0.64       633
           2       0.34      0.39      0.36       299
           3       0.36      0.35      0.35       385
           4       0.56      0.57      0.56       610
           5       0.34      0.33      0.34       961

    accuracy                           0.46      2888
   macro avg       0.45      0.45      0.45      2888
weighted avg       0.46      0.46      0.46      2888


🎯 LightGBM eğitiliyor... (SMOTE: Evet)
[LightGBM] [Info] Auto-choosing col-wise multi-threading, the overhead of testing was 0.107730 seconds.
You can set `force_col_wise=true` to remove the overhead.
[LightGBM] [Info] Total Bins 253852
[LightGBM] [Info] Number of data points in the train set: 19220, number of used features: 1130
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
[LightGBM] [Info] Start training from score -1.609438
/usr/local/lib/python3.11/dist-packages/sklearn/utils/validation.py:2739: UserWarning: X does not have valid feature names, but LGBMClassifier was fitted with feature names
  warnings.warn(
⏱️ Eğitim Süresi: 28.98 saniye
              precision    recall  f1-score   support

           1       0.67      0.64      0.66       633
           2       0.37      0.41      0.39       299
           3       0.40      0.35      0.37       385
           4       0.60      0.61      0.61       610
           5       0.39      0.40      0.39       961

    accuracy                           0.49      2888
   macro avg       0.49      0.48      0.48      2888
weighted avg       0.49      0.49      0.49      2888





📊 Karşılaştırma Tablosu:
                 Model  Accuracy  F1 Score  Training Time (s)  SMOTE  \
0              XGBoost  0.480263  0.480239          40.725557  Hayır   
1           Linear SVM  0.597645  0.594611           1.766109  Hayır   
2   LogisticRegression  0.388850  0.313150           9.295072  Hayır   
3         RandomForest  0.470222  0.465552          92.049367  Hayır   
4             LightGBM  0.499654  0.498365          13.951691  Hayır   
5              XGBoost  0.496537  0.497521          53.405068   Evet   
6           Linear SVM  0.561288  0.511474           3.407986   Evet   
7   LogisticRegression  0.426247  0.417844          18.665378   Evet   
8         RandomForest  0.474723  0.473693         266.374799   Evet   
9             LightGBM  0.517659  0.516832          24.154861   Evet   
10             XGBoost  0.361842  0.357589           7.311107  Hayır   
11          Linear SVM  0.506233  0.484962           4.642821  Hayır   
12  LogisticRegression  0.473684  0.453587          77.275234  Hayır   
13        RandomForest  0.342105  0.327194          17.471237  Hayır   
14            LightGBM  0.385388  0.378208           3.897743  Hayır   
15             XGBoost  0.366690  0.368758           9.031190   Evet   
16          Linear SVM  0.456717  0.422016           6.349095   Evet   
17  LogisticRegression  0.433172  0.415971          78.086202   Evet   
18        RandomForest  0.332410  0.324923          31.340207   Evet   
19            LightGBM  0.391620  0.391499           4.880553   Evet   
20             XGBoost  0.468144  0.468016          50.275709  Hayır   
21          Linear SVM  0.588643  0.585844          15.984710  Hayır   
22  LogisticRegression  0.469875  0.452208          22.615925  Hayır   
23        RandomForest  0.424515  0.409466         209.375416  Hayır   
24            LightGBM  0.480956  0.479807          19.001933  Hayır   
25             XGBoost  0.477147  0.478679          63.085433   Evet   
26          Linear SVM  0.579640  0.564676          22.644283   Evet   
27  LogisticRegression  0.432479  0.411514          39.064809   Evet   
28        RandomForest  0.455679  0.455660         511.175297   Evet   
29            LightGBM  0.492382  0.493028          28.984627   Evet   

      Feature Set  
0          TF-IDF  
1          TF-IDF  
2          TF-IDF  
3          TF-IDF  
4          TF-IDF  
5          TF-IDF  
6          TF-IDF  
7          TF-IDF  
8          TF-IDF  
9          TF-IDF  
10           BERT  
11           BERT  
12           BERT  
13           BERT  
14           BERT  
15           BERT  
16           BERT  
17           BERT  
18           BERT  
19           BERT  
20  BERT + TF-IDF  
21  BERT + TF-IDF  
22  BERT + TF-IDF  
23  BERT + TF-IDF  
24  BERT + TF-IDF  
25  BERT + TF-IDF  
26  BERT + TF-IDF  
27  BERT + TF-IDF  
28  BERT + TF-IDF  
29  BERT + TF-IDF  
