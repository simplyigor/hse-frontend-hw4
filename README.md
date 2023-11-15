### Описание 📝

**Выполнил:** Игорь Петров

Задание предполагает развертывание веб-приложения через любую облачную платформу / сервис для хостинга. В моем случае выбор пал на `Vercel`. В качестве веб-приложения я использовал верстку из [Задания №2](https://github.com/simplyigor/hse-frontend-hw1).

### "Многостраничность" 🗂️

Отображение нескольких страниц веб-приложения реализовано через [proxy](https://vercel.com/guides/how-can-i-serve-multiple-projects-under-a-single-domain):

```json
{
    "rewrites": [
      {"source": "/index", "destination": "https://hse-frontend-hw4.vercel.app"},
      {"source": "/tasks", "destination": "https://hse-frontend-hw4.vercel.app/tasks.html"},
      {"source": "/mentors", "destination": "https://hse-frontend-hw4.vercel.app/mentors.html"}
    ]
  }
```

### Тестирование 🤖

> [Cсылка](https://hse-frontend-hw4.vercel.app)
