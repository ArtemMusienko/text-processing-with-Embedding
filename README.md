![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)

## Text processing with Embedding

В данном коде представлен вариант обработки текста с использованием **токенизатора Razdel** и **слоем Embedding**. В качестве примера используется [датасет](https://storage.yandexcloud.net/academy.ai/russian_literature.zip) с текстами русских писателей и поэтов. Также будем использовать большую базу текстов на русском языке - **navec**.

Что же такое этот **Razdel** и **navec**?

**Razdel** — это эффективный токенизатор для русского языка, который точно разделяет текст на предложения и слова, корректно обрабатывая сложные случаи с точками, аббревиатурами и цифрами. В отличие от простого разбиения по пробелам, он понимает контекст и сохраняет целостность лексем.

**navec** — это большая предобученная модель векторных представлений слов (word embeddings) для русского языка, созданная на основе обширных текстовых корпусов. Эти эмбеддинги улавливают семантические и синтаксические связи между словами и используются как основа для решения задач NLP, таких как классификация текста или поиск синонимов.

Архитектура модели подробно описана в самом коде, а для достижения лучшего результата используются callbacks: **ModelCheckpoint**, **EarlyStopping** и **ReduceLROnPlateau**.

*Средняя точность распознавания: 90%*

> Настоятельно рекомендую использовать **графический ускоритель T4** или
> лучше для запуска кода!
