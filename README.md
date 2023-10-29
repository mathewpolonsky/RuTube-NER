# RuTube-NER  

Решение команды `Deviаnts` задачи NER от RuTube в рамках Хакатона [Цифровой прорыв](https://hacks-ai.ru).

Решение задачи извлечения именнованных сущностей (NER), представленное [`LaBSE-en-ru`](https://huggingface.co/cointegrated/LaBSE-en-ru). 

Перед обучением проведена тщательная разметка части датасета.

[Ссылка на csv с размеченными 1000 семплами](https://drive.google.com/file/d/1ZEtdNX2eo7gAuoiGHxQFYI50z3jJYH_q/view?usp=sharing)

## Стек решения
`Python`, `Transformers`, `PyTorch`

## Файлы  
[`wikineural_multilingual_ner.ipynb`](wikineural_multilingual_ner.ipynb) — обучение модели [`wikineural-multilingual_ner`](https://huggingface.co/Babelscape/wikineural-multilingual-ner)

[`Train_labse_and_submit.ipynb`](Train_labse_and_submit.ipynb) — обучение модели [`LaBSE-en-ru`](https://huggingface.co/cointegrated/LaBSE-en-ru) на 1000 наших семплов + остального датасета с изначальной разметкой. Создание сабмита
Для анализа кода обучения удобнее смотреть [`wikineural_multilingual_ner.ipynb`](wikineural_multilingual_ner.ipynb), так как он более чистый, финальный же ноутбук заполнен сумбурно

[`XLM_Roberta_Training.ipynb`](XLM_Roberta_Training.ipynb) — обучение [`xlm-roberta-large-finetunef-conll03`](https://huggingface.co/xlm-roberta-large-finetuned-conll03-english) и `xlm-roberta-large`
  
[`DeepPavlov.ipynb`](DeepPavlov.ipynb) — пробовали DeepPavlov для решения
