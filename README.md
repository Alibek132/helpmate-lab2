# HelpMate - Lab 2

HelpMate - статический многостраничный прототип платформы, где студенты могут публиковать анкеты и искать работу, а работодатели могут смотреть анкеты и размещать вакансии.

## Что выполнено

- Использованы только HTML и CSS, JavaScript отсутствует.
- Главный референс стиля: [Neumorphism](https://dummy.my/neumorphism) с сайта Dummy.my.
- Выбранная комбинация из Themes: **Neumorphism + Education & Learning**.
- Тема: светлый холодно-серый фон, синий акцент, мягкие внешние и внутренние тени. Для темной системной темы предусмотрена отдельная палитра.
- Все страницы используют единый файл `style.css`.
- Главные фотографии созданы специально для проекта и хранятся локально в папке `assets`.
- Реализованы адаптивные версии для компьютера, планшета и телефона.
- Добавлены темная системная тема, видимые состояния фокуса и поддержка `prefers-reduced-motion`.
- Все страницы связаны обычными HTML-ссылками.

## Страницы и endpoints

| Endpoint для презентации | HTML-файл | Назначение |
|---|---|---|
| `/home` | `index.html` | Главная страница и описание проекта |
| `/jobs` | `jobs.html` | Каталог вакансий для студентов |
| `/jobs/:id` | `job-details.html` | Полная информация о вакансии |
| `/students` | `students.html` | Каталог анкет студентов |
| `/students/:id` | `student-profile.html` | Профиль конкретного студента |
| `/post-job` | `post-job.html` | Форма публикации вакансии |
| `/post-resume` | `post-resume.html` | Форма создания анкеты студента |
| `/login` | `login.html` | Вход в аккаунт |
| `/register` | `register.html` | Регистрация студента или работодателя |
| `/profile` | `profile.html` | Личный профиль и статистика |
| `/applications` | `applications.html` | Список откликов и их статусы |
| `/messages` | `messages.html` | Переписка студента и работодателя |
| `/about` | `about.html` | Информация о проекте и безопасность |

Всего: **13 страниц**.

## Выбранные layouts

- Главная: [Sticky Header + Hero](https://dummy.my/layouts/hero-sticky-header/) и [Asymmetric Split](https://dummy.my/layouts/split-asymmetric/).
- Каталоги: [Card Grid](https://dummy.my/layouts/grid-card/) с фильтрами и боковой панелью.
- Детальная страница: [Asymmetric Split](https://dummy.my/layouts/split-asymmetric/) с основным контентом и блоком действия.
- Формы: [Settings / Profile Page](https://dummy.my/layouts/form-settings/) с двухколоночными полями.
- Авторизация: [Login / Auth](https://dummy.my/layouts/form-auth/) с центрированной карточкой.
- Профиль: [App Shell](https://dummy.my/layouts/dashboard-app-shell/) со статистикой и основным контентом.
- Сообщения: [Master-Detail](https://dummy.my/layouts/dashboard-master-detail/) со списком диалогов и открытым чатом.
- Базовая структура: [Header-Content-Footer Stack](https://dummy.my/layouts/classic-stacked/).

## Как объяснить CSS на защите

1. `:root` хранит общие переменные цветов, теней, радиусов и ширины контейнера.
2. `.container` ограничивает ширину контента и центрирует его.
3. `display: grid` используется для колонок, карточек и форм.
4. `display: flex` используется в навигации, кнопках и строках тегов.
5. Neumorphism создается двумя тенями: темной снизу справа и светлой сверху слева.
6. `box-shadow: inset` создает эффект вдавленного элемента для полей и фильтров.
7. `@media` меняет количество колонок и меню на небольших экранах.
8. `:hover`, `:active`, `:focus-visible` показывают реакцию элементов на действия пользователя.
9. Семантические теги `header`, `nav`, `main`, `section`, `article`, `aside`, `footer` описывают структуру страницы.

## Запуск

Откройте `index.html` в браузере или запустите простой локальный сервер в папке проекта.
