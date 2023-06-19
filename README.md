# API_Manual_Testing_Project

### **API** - Яндекс.Прилавок

### Чек-лист тестирования API:

[API Testing Checklist - Google Sheets](https://docs.google.com/spreadsheets/d/1p0yYjdk12BrvwguB1IXjkT76EPcaQK8QZqVwUTc5-W4/edit?usp=sharing "API Testing Checklist")

### Постановка задачи:
1. Проанализировать требования к новой функциональности бэкенда Яндекс.Прилавка и изучить документацию к API в Apidoc. [Требования к бэкенду.](https://praktikum.notion.site/8c91f759cb834ef2aa23db9d803a6373 "Требования к бэкенду в Notion")
2. Спроектировать тесты в виде чек-листа, чтобы покрыть следующие функциональности:
- Работа с наборами: 

  -возможность добавлять продукты в набор — POST /api/v1/kits/:id/products.
  
- Работа с курьерами:

  -возможность проверить, есть ли доставка курьерской службой «Привезём быстро» и сколько она стоит.POST /fast-delivery/v3.1.1/calculate-delivery.xml. 
 
- Работа с корзиной:
  -возможность получить список продуктов, которые добавили в корзину. GET /api/v1/orders/:id;
  
  -возможность добавлять продукты в корзину. PUT /api/v1/orders/:id;
  
  -возможность удалять корзину. DELETE /api/v1/orders/:id.
  
3. Протестировать API через Postman и завести баг-репорты в YouTrack.
