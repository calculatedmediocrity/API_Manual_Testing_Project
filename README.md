# API_Manual_Testing_Project

Тестирование API Яндекс.Прилавок использованием Postman

## Документация

1) API Testing Checklist - [Google Sheets](https://docs.google.com/spreadsheets/d/1p0yYjdk12BrvwguB1IXjkT76EPcaQK8QZqVwUTc5-W4/edit?usp=sharing "API Testing Checklist")

2) Коллекция Postman из 61 теста по работе с наборами - [Kits.postman_collection.json](https://github.com/calculatedmediocrity/API_Manual_Testing_Project/blob/main/Kits.postman_collection.json "collection")

3) Результат выполнения тестов - [Kits.postman_test_run.json](https://github.com/calculatedmediocrity/API_Manual_Testing_Project/blob/main/Kits.postman_test_run.json "test_run")

4) Бег-репорты https://prilavok.youtrack.cloud/issues

## Постановка задачи:
1. Проанализировать требования к новой функциональности бэкенда Яндекс.Прилавка и изучить документацию к API в Apidoc. 
2. Спроектировать тесты в виде чек-листа, чтобы покрыть следующие функциональности.
3. Оформить баг-репорты в Youtrack.

### - Работа с наборами: 

 <br> Возможность добавлять продукты в набор  </br>
 <br> POST /api/v1/kits/:id/products</br>

**Пример заголовков**
```
{
    "Content-Type": "application/json"
}
```

**Параметр**

| Название| Тип | Описание |
|----------|----------|----------|
|id  | number  | id набора в таблице kit_model. Передается урл-параметром |
| productList    | string  | productList набора. Массив, содержащий id продуктов и их количества. Передается в теле запроса. |
  
### - Работа с курьерами:

<br>Возможность проверить, есть ли доставка курьерской службой «Привезём быстро» и сколько она стоит</br>
<br>POST /fast-delivery/v3.1.1/calculate-delivery.xml</br>

**Пример заголовков**
```
{
    "Content-Type": "application/xml"
}
```

**Параметр**

| Название| Тип | Описание |
|----------|----------|----------|
|productsCount  | number  | Количество продуктов в заказе |
| productsWeight    | number  | Вес продуктов |
| deliveryTime    | number   |Планируемое время доставки |


 
