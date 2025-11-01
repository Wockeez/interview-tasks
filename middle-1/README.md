
## Тестовое задание: Angular Todo App с дополнительной функциональностью

### Основное задание (3-6 часов)
Создать приложение для управления задачами с следующими требованиями:

#### Функциональность:
1. **CRUD операции** с задачами (создание, просмотр, редактирование, удаление)
2. **Фильтрация** задач по статусу (все, активные, завершенные)
3. **Поиск** по названию задачи
4. **Сортировка** по дате создания/приоритету
5. **Локальное сохранение** данных (NGRX, NGXS) например - добавить задачу в избранное
6. **GMT+3** все даты/время должны быть конвертированы в часовой пояс GMT+3

#### Технические требования:
- Angular 15
- TypeScript (строгая типизация)
- Reactive Forms для создания/редактирования
- Валидация полей в соответствии с сервером
- RxJS для асинхронных операций
- Любой фреймворк для UI (**Разрешено всё** кроме [Angular Material](https://material.angular.dev/))
- Responsive дизайн

#### Структура задачи:
```typescript
interface Task {
  id: string;
  title: string;
  description?: string;
  priority: 'low' | 'medium' | 'high';
  status: 'pending' | 'completed';
  createdAt: Date;
  updatedAt: Date;
  dueDate?: Date;
}
```

### UI

На свое усмотрение, но в рамках контекста этой работы

- [Референс 1](https://screenshots.codesandbox.io/76ulz/69.png)
- [Референс 2](https://raw.githubusercontent.com/x1-il/todo-app/main/public/To-Do%20List%20_%20All%20tasks.png)
- [Референс 3](https://i.ytimg.com/vi/9_rveAI3eS4/maxresdefault.jpg)

### Backend API

Приложение должно использовать API которое указано ниже

Секция **Interview - Middle 1: TODO List**

[Swagger](https://evo-academy.wckz.dev/docs/middle-1)

### Дополнительные задачи (показать уровень):
1. **Drag & Drop** для изменения приоритета задач
2. **Виртуальный скроллинг** для большого списка задач
3. **Анимации** Angular Animations

### Временные рамки:
- **Основное задание**: 3-6 часов
- **С дополнительными задачами**: до 8 часов

### Результат:
Кандидат должен предоставить:
1. Исходный код (Git репозиторий)
2. README с инструкциями по запуску
3. Live demo (GitHub Pages/Netlify/Vercel/CodeSandbox) - по возможности
