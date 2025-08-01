# semantic-deduplication-sbert

This repository contains the result of a test assignment for an ML Engineer position.  
The task is focused on **semantic deduplication of product descriptions** using **SBERT embeddings** and **cosine similarity**.

---

## Контекст
Этот проект был выполнен в рамках тестового задания на позицию ML-инженера, связанного с задачей **семантического дедубликации карточек товаров**.

> **Формулировка задания:**  
> 1. Изучить предметную область.  
> 2. Выделить часть современных методов (SOTA) и оформить их в виде документа с логически последовательным изложением.  
> 3. Выбрать один из подходов, использующий косинусное сходство, и реализовать его на Python.

---

## Содержимое репозитория

| Файл                                      | Назначение                                                 |
|-------------------------------------------|------------------------------------------------------------|
| `SOTA дедупликация карточек товаров.pdf`  | Краткий обзор современных подходов на русском языке        |
| `e_commerce_deduplication_sbert.ipynb`    | Jupyter notebook с реализацией подхода на основе SBERT     |
| `ecommerce_products_ru.csv`               | Демонстрационный набор данных карточек товаров             |
| `requirements.txt`                        | Зависимости проекта                                        |

---

## Подход

- Модель `sbert_large_nlu_ru` с [huggingface](https://huggingface.co/ai-forever/sbert_large_nlu_ru)
- Косинусное сходство реализовано согласно формуле.
- Метрики качества: `precision`,`recall`,`F-мера`.
