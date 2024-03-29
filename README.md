# SemEval2024-task8-Subtask-B.

## Решение задачи классификации: "кто сгенерировал текст"

Текст может быть написан человеком или сгенерирован с помощью определенной языковой модели.   
## В ноутбуке `notebook-en-m.ipynb` - решение задачи для английского языка  
В качестве основных моделей использовались:
- `CatBoost` (0.96 f1-score)
   
  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/ddb074d8-96bd-4e9e-8d79-be37d5437c3e" width="400" />

- `BERT` (0.94 f1-score)

  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/40ab4086-2331-4859-b8bb-ae21d3e4e9fe" width="400" />
  
- `mBERT` (0.94 f1-score)
  
  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/9203d620-d245-4c9e-a14a-9a2a193ad528" width="400" />

- `xlm-roberta` (0.90 f1-score)

  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/77d9c796-0921-444f-9836-6670846253b0" width="400" />



# Так же был проведен `EDA` 

   ![image](https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/467a2fe8-bec2-4250-bf10-9f5ab431e65f)

`PCA` и `tf-idf`           |  Распределение длинн текстов в словах и в символах
:-------------------------:|:-------------------------:
![image](https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/95fb5fb5-6c3a-4d27-89ee-64e7653fd0d3)  |  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/230738e2-6b76-47d2-80d5-2e17c79afbf2" width="300" /> <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/6d7b0e83-1d7d-4c29-9162-6c2c3aa61f20" width="300" />





   ![image](https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/769588fd-b851-49c4-93dc-e1d3f7a814b1)


Выделив топ 25 фич c помощью F-теста видим, что наличие и число ссылок (фичи - `external links` и `references`) имеет одну из самых больштих корелляций, что забавно, так как у ИИ проблемы с указанием ссылок
## В ноутбуке `notebook_multi_m.ipynb`- решение задачи для разных языков
Основные модели:
- `CatBoost` (0.94 f1-score)

   <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/af33954d-7d71-4a61-abcb-a7c67ab34ac9" width="400" />

- `DistilmBERT` (0.96 f1-score)

  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/18f8b058-4b57-4ac5-9de8-dfc3e8e98101" width="400" />
  
- `mBERT` (0.95 f1-score)

  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/9df089eb-debc-4783-9535-45316f6eb520" width="400" />

- `xlm-roberta` (0.95 f1-score)

  <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/21ca5714-54de-4de3-ac96-a7dd31d7515a" width="400" />

# Визуализация `tf-idf`+ `PCA`

Для разных языков визуализация выглядит не очень информатично, так как выделились несколько групп языков

`PCA` и `tf-idf`           |  Распределение длинн текстов в словах и в символах
:-------------------------:|:-------------------------:
![image](https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/dbc4b118-95df-4a50-b1f2-3e3cc418177e) | <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/fbd60e0f-e99e-40aa-81a4-7d20d6811791" width="300" /> <img src="https://github.com/BerezinDaniil/SemEval2024-task8-Subtask-B/assets/78606208/da753871-3627-4bf8-8cc0-1350a8cbb533" width="300" />

