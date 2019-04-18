# MyCoin - Баг трекер

## Сборки

Статус стабильной сборки (master): [![Netlify Status](https://api.netlify.com/api/v1/badges/ff3928cd-6fe8-4980-9dba-7cb4de249332/deploy-status)](https://app.netlify.com/sites/nostalgic-dijkstra-86999e/deploys)

Статус тестовой сборки (test): Не выпущена

## Инструкции по созданию отчетов в баг-трекере

- Создавать отчеты можно [здесь](https://github.com/skritt3/MyCoinIssues/issues) используя кнопку "New Issue"

### Правила создания отчетов:

1. **Заголовок:**
* В заголовке необходимо одним предложением передать суть найденного бага или пожелания. Краткая выжимка, по которой разработчик и каждый из команды сможет понять, в чем дело. 
Хороший заголовок: «Список сообществ в подписках пуст». 
Плохой заголовок: «Нет сообществ». Откровенно плохой: «Странная заглушка». Избегайте неопределенности. Разработчик, модератор или руководитель проекта (а иногда все вместе взятые) при не информативном заголовке потратят много времени, чтобы открыть отчет, и уже по описанию понять, о чем речь.
2. **Описание**
* Описание бага должно состоять из одной опциональной (предварительные условия) и трех обязательных частей: шаги воспроизведения, фактический результат, ожидаемый результат. 
3. **Файлы:**
* Наиболее популярная сущность вложений. Скриншоты сообщений об ошибке, багов верстки, грамматических и орфографических ошибок, локализации и интернационализации обязательны. В остальных случаях опциональны, но считаются правилом хорошего тона. Именно скриншоты, а не фото экрана. Фото экрана - крайний случай, когда скриншот сделать невозможно никаким способом. 
4. **Структура:**
* Все отчеты должны быть составлены **четко** по структуре которая описана ниже.
5. **Важные категории:**
* **Дубликаты**:
  + Перед тем, как создать отчет, убедись, что баг не зарепортил кто-нибудь другой. Если отчет о баге или предложение уже есть в трекере, лучше оставить комментарий с деталями к существующему отчету, чем множить дубликаты. Отчет об уже заведенном баге стоит создавать только когда вы абсолютно уверены, что первоначальный не несет в себе никакой информационной стоимости, но в этом случае укажите ссылку на него.
* **Уязвимости**
  + Уязвимости оцениваются выше и рассматриваются отдельно, во избежание эксплуатации не отображаются другим тестировщикам в проекте, поэтому правила о дубликатах на платформе бета-тестирования на них не распространяются.  
* **Пожелания**
  + Помимо отчета о баге есть и другая сущность - пожелание. К этому типу отчетов относятся запросы на реализацию фичи, предложения по улучшению интерфейса, удобства использования и производительности.  
  + В **пожеланиях** обязательным является детальное описание текущей работы или состояния приложения, путь к экрану/странице/функциональности, которая по вашему мнению нуждается в изменении, и желаемый результат.

### Структура отчета:

**Устройство:** Устройство на котором произошел баг (Например: Samsung Galaxy Note 9/IPhone XS)

**Платформа:** Платформа на которой произошел баг (IOS/ANDROID).

**Версия платформы**: Версия платформы (Например: 9.0)

**Сборка**: Кодовое название сборки из списка сверху на которой произошел баг (Например: master)

**VK ID**: ID вашей страницы ВКонтакте на которой был воспроизведен баг

**Предварительные условия (preconditions):**
  + Опционально. То, что нужно сделать перед выполнением шагов воспроизведения. Возможно, создать аккаунт пользователя с разными значениями полей, или ограничить пропускную способность канала. 

**Шаги воспроизведения:**
  + Должны быть равновесными, необходимыми и достаточными для воспроизведения проблемы. 

   + Например: 
      1) Запустить приложение и авторизоваться c помощью VK (oauth.vk.com). 
      2) Перейти на вкладку ленты в таббаре. 
      3) Нажать на иконку подписок в верхнем левом углу. 
      4) Тап по вкладке “Сообщества” в segmented control. Список сообществ отображается пустым. 
      5) Нажать кнопку добавления (+) на экране подписок. 
      6) Повторить шаг #4. 
  
**Фактический результат:** То, что наблюдаем после выполнения последнего шага.

**Ожидаемый результат:** То, что мы ожидаем увидеть.

**Приоритет:**
  + Критичность бага с точки зрения тестировщика и продукта в целом. 
На нашей платформе существуют четыре приоритета:
Критический - баги, блокирующие дальнейшую работу приложения или дальнейшее тестирование, падения, зависания, потеря или порча пользовательских данных.
    + Высокий - неработающая функциональность, или работающая неверно. Например, не отправить сообщение, не удалить фотографию.
    + Средний - баг не критично влияет на продукт, но доставляет существенные неудобства; фича работает некорректно, но существует workaround - действие можно выполнить другим способом.
    + Низкий - баги, не нарушающие бизнес-логику, с незначительным влиянием на продукт в целом, проблемы с отображением элементов и     данных на экране, грамматические и орфографические ошибки.
    
**P.S. Некоторые категории могут не использоваться в зависимости от вида отчета (Баг/Пожелание и т.д.)**

### Пример отчета:

![Screenshot_1](https://user-images.githubusercontent.com/25477504/56364633-ab48c480-61f7-11e9-84d2-7c7d3c2a396c.png)

### Текстовая версия примера отчета с разметкой:

```
- **Устройство:** Samsung Galaxy S8
- **Платформа:** Android
- **Версия платформы** 9.0
- **Сборка:** master
- **Предварительные условия (preconditions):** -

- **Шаги воспроизведения:**

      1. Войти в приложение
      2. Открыть раздел "Топ"
      3. Нажать вкладку "Сообщества"

- **Фактический результат:** Во вкладке "Сообщества" наблюдаем список друзей, а во вкладке "Друзья" не наблюдаем ничего.

- **Ожидаемый результат:** Во вкладке "Друзья" наблюдаем список друзей, а во вкладке "Сообщества" не наблюдаем ничего, так как функционал не реализован.

- **Приоритет:** Средний

- **Скриншоты:**
![jsq4LGY3CN0](https://user-images.githubusercontent.com/25477504/56364372-0b8b3680-61f7-11e9-9701-6e3e080037c1.jpg)
```

## RoadMap

- [x] Реализация базового дизайна
- [x] Реализация разделов
- [x] Реализация связи с БД
- [x] Реализация блокировок
- [x] Реализация общего топа
- [ ] Реализация топа друзей
- [ ] Реализация оффлайн уведомления
- [ ] Реализация переводов
- [ ] Исправление кнопок
- [ ] Реализация онлайна с одного устройства
- [ ] Выпуск бета сборки (test) для поэтапного выпуска обновлений и закрытие публичного доступа к сборкам
- [ ] Реализация счетчика коинов/сек и его связь с БД
- [ ] Добавление коинов/сек в реальном времени
- [ ] Реализация и добавление первого улучшения
- [ ] Реализация кликов
- [ ] Реализация счетчика онлайна
- [ ] Рефакторинг
