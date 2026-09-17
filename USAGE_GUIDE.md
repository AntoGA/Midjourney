# Полное Руководство по Использованию

Детальное руководство по использованию коллекции навыков для редакционной фотографии в Midjourney.

---

## Содержание

1. [Быстрый Старт](#быстрый-старт)
2. [Основы Midjourney](#основы-midjourney)
3. [Структура Промптов](#структура-промптов)
4. [Параметры и Настройки](#параметры-и-настройки)
5. [Работа со Стилями](#работа-со-стилями)
6. [Практические Примеры](#практические-примеры)
7. [Продвинутые Техники](#продвинутые-техники)
8. [Устранение Проблем](#устранение-проблем)
9. [Рабочие Процессы](#рабочие-процессы)
10. [Ресурсы](#ресурсы)

---

## Быстрый Старт

### 1. Выберите Стиль

Откройте `editorial_skills.md` или `editorial_skills_extended.md` и выберите стиль фотографа, который вам нужен.

### 2. Скопируйте Базовый Промпт

Каждый навык содержит готовый промпт с плейсхолдером `[SUBJECT]`.

### 3. Замените [SUBJECT]

Замените `[SUBJECT]` на описание вашего объекта:

```
До:  Editorial portrait photography in the style of Annie Leibovitz, [SUBJECT], dramatic cinematic lighting...
После: Editorial portrait photography in the style of Annie Leibovitz, a tech CEO in modern office, dramatic cinematic lighting...
```

### 4. Вставьте в Midjourney

Вставьте промпт в Discord бот Midjourney или на веб-сайте.

---

## Основы Midjourney

### Что такое Midjourney?

Midjourney — это AI-генератор изображений, который создает фотографии по текстовому описанию (промпту).

### Версии

- **v6** — последняя версия с максимальным качеством (рекомендуется)
- **v5.2** — предыдущая стабильная версия
- **niji** — специализированная версия для аниме и иллюстраций

### Доступ

- Discord бот (основной способ)
- Веб-интерфейс (alpha.midjourney.com)
- API (для разработчиков)

---

## Структура Промптов

### Базовая Структура

```
[СТИЛЬ] + [ОБЪЕКТ] + [ТЕХНИЧЕСКИЕ ДЕТАЛИ] + [ПАРАМЕТРЫ]
```

### Компоненты Промпта

#### 1. Стиль Фотографа
```
in the style of Annie Leibovitz
inspired by Peter Lindbergh
```

#### 2. Описание Объекта
```
a tech CEO in modern office
elderly craftsman in workshop
model in red couture gown
```

#### 3. Технические Детали
```
shot on Hasselblad H6D-100c, 80mm lens, f/2.8
dramatic cinematic lighting
shallow depth of field
```

#### 4. Параметры Midjourney
```
--ar 3:2          # Соотношение сторон
--style raw       # Минимальная стилизация
--v 6             # Версия
--q 2             # Качество
```

---

## Параметры и Настройки

### Соотношение Сторон (--ar)

| Параметр | Формат | Использование |
|----------|--------|---------------|
| `--ar 1:1` | Квадрат | Социальные сети, аватары |
| `--ar 3:2` | Горизонтальный | Журналы, документальная |
| `--ar 2:3` | Вертикальный | Fashion editorial |
| `--ar 4:5` | Портрет | Журнальные портреты |
| `--ar 16:9` | Широкоэкранный | Кинематограф |
| `--ar 21:9` | Ультраширокий | Панорамы |

### Стиль (--style)

| Параметр | Эффект | Когда использовать |
|----------|--------|-------------------|
| `--style raw` | Минимальная стилизация | Реалистичная фотография |
| `--style cute` | Мягкий стиль | Иллюстрации |
| `--style expressive` | Экспрессивный | Арт-проекты |

### Качество (--q)

| Параметр | Время | Качество |
|----------|-------|----------|
| `--q 0.25` | Быстро | Черновик |
| `--q 0.5` | Средне | Стандарт |
| `--q 1` | Долго | Высокое |
| `--q 2` | Очень долго | Максимальное |

### Версия (--v)

```
--v 6      # Последняя версия (рекомендуется)
--v 5.2    # Предыдущая стабильная
--v 4      # Старая версия
```

### Дополнительные Параметры

```
--no [слово]        # Исключить элемент
--chaos 50          # Вариативность (0-100)
--stylize 100       # Степень стилизации (0-1000)
--seed 12345        # Фиксированный seed для воспроизводимости
--tile              # Создать паттерн
--cw 100            # Вес изображения (0-100)
```

---

## Работа со Стилями

### Выбор Стиля по Задаче

#### Журнальная Публикация
- **Annie Leibovitz** — обложки, celebrity portraits
- **Mario Testino** — fashion editorial
- **Richard Avedon** — минималистичные портреты

#### Документальная Фотография
- **Steve McCurry** — культурные портреты
- **Henri Cartier-Bresson** — уличная фотография
- **Dorothea Lange** — социальная документалистика

#### Fashion и Реклама
- **Tim Walker** — сюрреалистичная fashion
- **Helmut Newton** — провокационная fashion
- **Juergen Teller** — сырая fashion

#### Арт-Проекты
- **Gregory Crewdson** — кинематографические сцены
- **Andreas Gursky** — монументальные пейзажи
- **Cindy Sherman** — концептуальные портреты

### Комбинирование Стилей

#### Метод 1: Последовательное Применение
```
Editorial portrait photography combining the dramatic lighting of Annie Leibovitz 
with the raw emotion of Peter Lindbergh, [SUBJECT]...
```

#### Метод 2: Гибридный Подход
```
Fashion editorial photography inspired by Tim Walker's surrealism 
and Mario Testino's vibrant colors, [SUBJECT]...
```

#### Метод 3: Контрастные Стили
```
Documentary photography blending Steve McCurry's rich colors 
with Henri Cartier-Bresson's decisive moment, [SUBJECT]...
```

---

## Практические Примеры

### Пример 1: Портрет Бизнесмена

**Задача:** Создать портрет CEO для журнала Forbes

**Выбор стиля:** Annie Leibovitz (environmental portraiture)

**Промпт:**
```
Editorial portrait photography in the style of Annie Leibovitz, 
a tech CEO in modern glass office, dramatic cinematic lighting, 
rich color palette, environmental storytelling, theatrical composition, 
medium format camera quality, shallow depth of field, professional 
studio lighting with natural elements, shot on Hasselblad H6D-100c, 
80mm lens, f/2.8 --ar 3:2 --style raw --v 6
```

### Пример 2: Fashion Editorial

**Задача:** Создать fashion-снимок для Vogue

**Выбор стиля:** Tim Walker (surreal fashion fantasy)

**Промпт:**
```
Surreal fashion editorial photography in the style of Tim Walker, 
model surrounded by oversized flowers in enchanted garden, whimsical 
fantasy elements, dreamlike atmosphere, pastel color palette, elaborate 
props, theatrical staging, shot on Hasselblad X2D 100C, 90mm lens, 
f/5.6, soft diffused lighting, magical realism, couture fashion, 
otherworldly beauty --ar 2:3 --style raw --v 6
```

### Пример 3: Документальный Портрет

**Задача:** Создать портрет ремесленника для National Geographic

**Выбор стиля:** Steve McCurry (documentary color)

**Промпт:**
```
Documentary editorial photography in the style of Steve McCurry, 
traditional potter in workshop surrounded by clay vessels, rich 
saturated colors, cultural authenticity, piercing eye contact, 
environmental context, storytelling composition, shot on Nikon Z9, 
85mm f/1.4 lens, natural window light, vibrant textiles, human 
connection, photojournalistic integrity --ar 3:2 --style raw --v 6
```

### Пример 4: Уличная Фотография

**Задача:** Запечатлеть городской момент

**Выбор стиля:** Henri Cartier-Bresson (decisive moment)

**Промпт:**
```
Street photography in the style of Henri Cartier-Bresson, man 
jumping over puddle in Parisian street, decisive moment, geometric 
composition, black and white, candid photography, 35mm film aesthetic, 
natural light, urban environment, spontaneous action, perfect timing, 
shot on Leica M3, 50mm Summicron lens, f/8, documentary photography, 
human interest --ar 3:2 --style raw --v 6
```

---

## Продвинутые Техники

### 1. Детализация Объекта

#### Базовое Описание
```
a woman in red dress
```

#### Детальное Описание
```
a confident woman in her 30s wearing elegant red silk evening gown, 
standing in grand marble hallway, golden chandeliers above, polished 
stone floors reflecting light, classical architecture columns
```

### 2. Контроль Освещения

#### Типы Освещения
```
natural window light          # Естественный свет из окна
golden hour lighting          # Золотой час (закат/рассвет)
dramatic cinematic lighting   # Драматическое кинематографическое
soft diffused lighting        # Мягкий рассеянный свет
hard flash lighting           # Жесткая вспышка
available light               # Доступный свет
studio lighting setup         # Студийное освещение
```

### 3. Технические Спецификации

#### Камеры
```
Hasselblad H6D-100c           # Средний формат, 100MP
Phase One XF IQ4 150MP        # Средний формат, 150MP
Leica M10 Monochrom           # Дальномерная, ч/б
Nikon Z9                      # Полнокадровая зеркалка
Canon EOS R5                  # Полнокадровая беззеркалка
8x10 large format camera      # Большой формат
```

#### Объективы
```
35mm lens                     # Широкоугольный
50mm lens                     # Стандартный
85mm lens                     # Портретный
110mm lens                    # Средний телеобъектив
300mm lens                    # Телеобъектив
```

#### Диафрагма
```
f/1.4                         # Очень широкая (боке)
f/2.8                         # Широкая (портреты)
f/5.6                         # Средняя
f/8                           # Оптимальная резкость
f/16                          # Узкая (пейзажи)
f/32                          # Очень узкая (максимальная ГРИП)
```

### 4. Использование Seed

Для воспроизводимости результатов:

```
[промпт] --seed 12345
```

Сохраните seed для создания вариаций:

```
[тот же промпт] --seed 12345 --chaos 20
```

### 5. Итеративное Улучшение

#### Шаг 1: Базовый Промпт
```
Editorial portrait of a musician, dramatic lighting --ar 3:2 --v 6
```

#### Шаг 2: Добавить Детали
```
Editorial portrait of a jazz musician with saxophone, dramatic 
cinematic lighting, smoky club atmosphere --ar 3:2 --style raw --v 6
```

#### Шаг 3: Полный Промпт
```
Editorial portrait photography in the style of Annie Leibovitz, 
jazz musician with vintage saxophone in smoky club, dramatic 
cinematic lighting, rich color palette, environmental storytelling, 
shot on Hasselblad H6D-100c, 80mm lens, f/2.8 --ar 3:2 --style 
raw --v 6 --q 2
```

### 6. Вариации и Upscale

#### Создание Вариаций
После генерации используйте кнопки V1-V4 для создания вариаций понравившегося варианта.

#### Upscale
Используйте U1-U4 для увеличения разрешения выбранного изображения.

### 7. Негативные Промпты

Исключите нежелательные элементы:

```
[промпт] --no text, watermark, signature, low quality
```

### 8. Весовые Коэффициенты

Приоритет элементов в промпте:

```
editorial portrait::2 dramatic lighting::1.5 red dress::1
```

---

## Устранение Проблем

### Проблема: Изображение Слишком Стилизованное

**Решение:**
```
Добавьте: --style raw
Уменьшите: --stylize 50 (вместо 100)
```

### Проблема: Недостаточная Детализация

**Решение:**
```
Увеличьте: --q 2
Добавьте: конкретные камеры и объективы
Добавьте: больше деталей в описание объекта
```

### Проблема: Неправильное Соотношение Сторон

**Решение:**
```
Проверьте параметр --ar
Используйте правильные значения: 3:2, 4:5, 16:9
```

### Проблема: Изображение Не Реалистичное

**Решение:**
```
Добавьте: shot on [конкретная камера]
Добавьте: [конкретный объектив] lens
Добавьте: f/[значение диафрагмы]
Добавьте: [тип освещения]
```

### Проблема: Слишком Много Элементов

**Решение:**
```
Упростите описание объекта
Используйте --no для исключения
Разбейте на несколько генераций
```

### Проблема: Повторяющиеся Результаты

**Решение:**
```
Измените seed: --seed [новое число]
Увеличьте chaos: --chaos 50
Добавьте вариации в описание
```

---

## Рабочие Процессы

### Рабочий Процесс 1: Журнальная Публикация

1. **Брифинг**
   - Определите тему статьи
   - Выберите целевую аудиторию
   - Определите тон и стиль

2. **Выбор Стиля**
   - Annie Leibovitz для celebrity
   - Mario Testino для fashion
   - Steve McCurry для документальной

3. **Создание Промпта**
   - Детальное описание объекта
   - Технические спецификации
   - Параметры Midjourney

4. **Генерация**
   - Создайте 4-8 вариантов
   - Выберите лучшие
   - Создайте вариации

5. **Финализация**
   - Upscale выбранного варианта
   - Постобработка в Photoshop
   - Подготовка к публикации

### Рабочий Процесс 2: Fashion Editorial

1. **Концепция**
   - Тема коллекции
   - Настроение и атмосфера
   - Цветовая палитра

2. **Выбор Стиля**
   - Tim Walker для сюрреализма
   - Helmut Newton для провокации
   - Juergen Teller для raw эстетики

3. **Подготовка**
   - Описание одежды и аксессуаров
   - Локация и декорации
   - Позы и выражения

4. **Генерация**
   - Серия из 5-10 изображений
   - Разные ракурсы и композиции
   - Вариации освещения

5. **Сборка**
   - Выбор лучших кадров
   - Создание последовательности
   - Финальная коррекция

### Рабочий Процесс 3: Документальный Проект

1. **Исследование**
   - Тема и контекст
   - Историческая справка
   - Визуальные референсы

2. **Выбор Стиля**
   - Henri Cartier-Bresson для улицы
   - Dorothea Lange для социальной темы
   - Sebastião Salgado для эпического масштаба

3. **Планирование**
   - Локации и ситуации
   - Типы субъектов
   - Временные рамки

4. **Генерация**
   - Разнообразие сцен
   - Естественные моменты
   - Экологические портреты

5. **Редактирование**
   - Отбор лучших кадров
   - Создание нарратива
   - Добавление контекста

---

## Ресурсы

### Официальные Ресурсы Midjourney

- **Документация:** https://docs.midjourney.com
- **Discord:** https://discord.gg/midjourney
- **Галерея:** https://www.midjourney.com/showcase

### Обучение

- **Midjourney Academy:** Официальные обучающие материалы
- **YouTube:** Каналы с туториалами
- **Reddit:** r/midjourney сообщество

### Вдохновение

- **Instagram:** Аккаунты фотографов
- **Magazines:** Vogue, Vanity Fair, National Geographic
- **Museums:** Онлайн-коллекции MoMA, Tate, Guggenheim

### Инструменты

- **Prompt Generators:** Онлайн-генераторы промптов
- **Image Editors:** Photoshop, Lightroom, Capture One
- **Organization:** Notion, Airtable для управления проектами

---

## FAQ

### Q: Какую версию Midjourney использовать?
**A:** Всегда используйте последнюю версию (v6) для максимального качества.

### Q: Можно ли использовать для коммерческих целей?
**A:** Да, если у вас платная подписка Midjourney.

### Q: Как сохранить консистентность в серии?
**A:** Используйте одинаковый seed и похожие промпты для всех изображений.

### Q: Как улучшить качество портретов?
**A:** Добавляйте конкретные камеры, объективы и параметры диафрагмы.

### Q: Можно ли комбинировать стили?
**A:** Да, экспериментируйте с комбинациями для уникальных результатов.

### Q: Как избежать артефактов?
**A:** Используйте --style raw и избегайте слишком сложных промптов.

---

## Заключение

Эта коллекция предоставляет вам профессиональные инструменты для создания изображений редакционного качества. Экспериментируйте, комбинируйте стили и развивайте свое уникальное видение.

**Ключевые Принципы:**
- Детализация описания объекта
- Технические спецификации камер и объективов
- Правильные параметры Midjourney
- Итеративное улучшение
- Эксперименты и творчество

Удачи в создании потрясающих изображений!
