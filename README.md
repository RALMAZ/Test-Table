# Test table
  
<p align="center">
<img src="https://s22.postimg.cc/e32adqepd/preview.png">
</p>  

    
1) Реализовать таблицу с 4 полями:
- Порядковый номер,
- Чекбокс "очистить" (по-умолчанию unselected)
- Название
- Вес
2) Заполнить данными
data: [
        { id: 1, title: 'Яблоко', weight: 4},
        { id: 2, title: 'Груша', weight: 7},
        { id: 3, title: 'Слива', weight: 1},
]
3) Таблица реализована разными темплейтами (потомками):
- table
- tableCell
- checkbox
4) При выборе пользователем чекбокса (перевод в состояние selected) :
    4.1. Заполнить все поля текущей строки значением '-', кроме поля порядковый номер
    4.2. Маркировать бордер текущей строки красным
5) При отмене ранее выбранного чекбокса (переводе в состояние unselected):
    5.1. Значение полей текущей строки вернуть к исходным.
    5.2. Убрать красную маркировку бордера
  
  
## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```
