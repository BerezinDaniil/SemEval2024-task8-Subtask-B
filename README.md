idf# SemEval2024-task8-Subtask-B.

## Решение задачи классификации: "кто сгенерировал текст"

Текст может быть написан человеком или сгенерирован с помощью определенной языковой модели.

В качестве основных моделей использовались:
- `CatBoost` (0.96 f1-score)
- `BERT` (0.94 f1-score)
- `mBERT` (0.94 f1-score)
- `xlm-roberta` (0.90 f1-score)


Так же был проведен `EDA` с применением `PCA` и `tf-idf` векторайзера 

![image](https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/95fb5fb5-6c3a-4d27-89ee-64e7653fd0d3)

Выделив топ 25 фич c помощью F-тест
![image](https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/769588fd-b851-49c4-93dc-e1d3f7a814b1)

видим, что наличие ссылок имеет одну из самых больштих корелляций, что забавно, так как у ИИ проблемы с указанием ссылок
