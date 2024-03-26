# SemEval2024-task8-Subtask-B.

## Решение задачи классификации: "кто сгенерировал текст"

Текст может быть написан человеком или сгенерирован с помощью определенной языковой модели.

В качестве основных моделей использовались:
- `CatBoost` (0.96 f1-score)
   
  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/ddb074d8-96bd-4e9e-8d79-be37d5437c3e" width="400" />

- `BERT` (0.94 f1-score)

  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/40ab4086-2331-4859-b8bb-ae21d3e4e9fe" width="400" />
  
- `mBERT` (0.94 f1-score)
  
  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/9203d620-d245-4c9e-a14a-9a2a193ad528" width="400" />

- `xlm-roberta` (0.90 f1-score)

  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/77d9c796-0921-444f-9836-6670846253b0" width="400" />



# Так же был проведен `EDA` с применением `PCA` и `tf-idf` векторайзера 

![image](https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/95fb5fb5-6c3a-4d27-89ee-64e7653fd0d3)


![image](https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/769588fd-b851-49c4-93dc-e1d3f7a814b1)


Выделив топ 25 фич c помощью F-теста видим, что наличие ссылок имеет одну из самых больштих корелляций, что забавно, так как у ИИ проблемы с указанием ссылок
