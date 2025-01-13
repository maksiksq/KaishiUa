# KaishiUa 1.5k

Вітаю у публічній репозиторії українського перекладу **Kaishi 1.5k** - сучасної колоди Anki створеної, щоб дозволити початківцям отримати базовий японський словниковий запас і якнайприємніше розпочати ваше вивчення японської мови.

Ось так виглядає передня сторона колоди:

<img src="https://github.com/maksiksking/KaishiUa/blob/main/pics/kaishi-front.png" alt="Передня частина картки KaishiUa 1.5k" style="width: 100%; height: auto">

Ось вивчаємо слово і речення до цього слова. Далі відкриваємо карточку, і на задній стороні бачимо його значення та переклад речення:

<img src="https://github.com/maksiksking/KaishiUa/blob/main/pics/kaishiua-back.png" alt="Задня частина картки KaishiUa 1.5k" style="width: 100%; height: auto"> 
Обираєш чи ти знаєш, чи пам'ятаєш це слово, повторюєш і починаєш вивчати, по трошки.

### Зміст цієї сторінки

- [Де мені отримати колоду?](#де-мені-отримати-колоду)
- [Що? Де? Коли?](#що-де-коли)
- [Інші пов'язані колоди та ресурси](#інші-повязані-колоди-та-ресурси)
- [Налаштування колоди](#налаштування-колоди)
- [Трошки про колоду](#трошки-про-колоду)
- [Помилки та пропозиції](#помилки-та-пропозиції)
- [Подяки](#подяки)

## Де мені отримати колоду?

Щоб використовувати потрібно мати чи встановити [Anki](https://apps.ankiweb.net/), після цього можна змінити інтерфейс на українську (ctrl+p і там Language), або цього не робити. Далі встановити .apkg файл зі сторінки [релізів](https://github.com/maksiksking/KaishiUa/releases) чи з [AnkiWeb](https://ankiweb.net/shared/info/871374951?cb=1736783944302), і імпортувати колоду кнопкою `Імпортувати файл` -> `Імпорт`. Далі використовувати, як саме описано далі.

## Що? Де? Коли?

Щоб почати веселитись і травмуватися з колодою потрібно знати хірагана та катакана, двоє з трьох японських систем написання, третя це канджі яких отут якраз сповно. Нормальних україномовних ресурсів для перших двох поки не існує, але я рекомендую [оцю](https://ankiweb.net/shared/info/1081858108) колоду для хірагана, і [ось](https://ankiweb.net/shared/info/1027153995) для катакана.

Щоб учитися потрібно зайти в Anki та імпортувати колоду, далі вся суть у тому, щоб подивитися на верх карточки, подумати чи ти пам'ятаєш значення і вимову слова та натиснути `Показати відповідь`, якщо ти знав це слово - вітаю, це потужно, просто перемога, натискай `Добре`, а якщо не знав, це поразка, але так зі всіма словами на початку, натискай `Знову`. Також можна використовувати кнопки `Тяжко` та `Легко` на ваш розсуд. 

Кількість нових карток у день можна змінити в налаштуваннях колоди, спочатку брати надто багато слів і потім їх повторювати цілий день це дуже поширена помилка, тому по трошки і залежно від вашого часу. 

Коли ваші картки доходять до деякого інтервалу який ви вирішуйте самі (наприклад 2 роки), і ви бажаєте, щоб Anki більше вам не показував цю карту натискайте shift+1, щоб її призупинити, тобто порізати її на капусту. Якщо це було необдумане рішення, то повернути її можна за допомогою ctrl+z чи у меню `Навігатор`. І далі продовжуємо так доки не призупинили всі картки, або вважаєте, що ви вивчили усе, що вам потрібно.

Те, що я описав це лиш один спосіб користуватись Anki, але насправді головне це вчитися, і ви можете робити, що хочете якщо ви знаєте, що ви не покинете колоду і головне продовжите вивчати японську.

## Інші пов'язані колоди та ресурси

А пов'язаних колод нема. На жаль, це одна з небагатьох україномовних колод Anki, але можливо саме ти зможеш перекласти чи створити свою колоду, щоб допомогти розвитку (і існуванню) українського япономовного ком'юніті. 

Скоро тут також з'являться ресурси для вивчення хірагана та катакана, але поки що рекомендую вищезазначені колоди.

## Налаштування колоди

Є кілька опцій, всі вони не обов'язкові, щоб змінити їх натисніть `Навігатор`, виберіть будь-яку карту та натисніть справа зверху `Картки...` і потім `Шаблон зворотньої сторони` чи двоє інших.

<details>
<summary>Налаштування</summary>
	
### Інтонаційні наголоси

Ви можете ввімкнути інтонаційні наголоси. Чи потрібно їх вивчати, чи ні це за вами, але якогось однорідного рішення від англомовного ком'юніті чи це справді потрібно немає.

```CSS
<div lang="ja">
{{furigana:Word Furigana}}

<!-- Це вмикає інтонаційні наголоси.

{{#Pitch Accent}}
	<br><div style='font-size: 24px'>{{Pitch Accent}}</div>
{{/Pitch Accent}} 

-->

<div style='font-size: 25px; padding-bottom:20px'>{{Word Meaning}}</div>
<div style='font-size: 25px;'>{{furigana:Sentence Furigana}}</div>
<div style='font-size: 25px; padding-bottom:10px'>{{Sentence Meaning}}</div>

{{Word Audio}}
{{Sentence Audio}}
<br>
{{Picture}}

{{#Notes}}
	<br>
	<div style="font-size: 20px; padding-top:12px">Примітка: {{Notes}}</div>
{{/Notes}}

<!-- Це вмикає примітки до інтонаційних наголосів.

{{#Pitch Accent Notes}}
<div style="font-size: 20px; width: fit-content; max-width:40vw; margin: auto">
	<details><summary>Примітка до Інтонаційних Наголосів:</summary>
		<br>{{Pitch Accent Notes}}
	</details>
</div>
{{/Pitch Accent Notes}}

-->

</div>
```

Щоб їх ввімкнути потрібно забрати `<!--` і `-->` ось так: 

```CSS
<div lang="ja">
{{furigana:Word Furigana}}

{{#Pitch Accent}}
	<br><div style='font-size: 24px'>{{Pitch Accent}}</div>
{{/Pitch Accent}} 

<div style='font-size: 25px; padding-bottom:20px'>{{Word Meaning}}</div>
<div style='font-size: 25px;'>{{furigana:Sentence Furigana}}</div>
<div style='font-size: 25px; padding-bottom:10px'>{{Sentence Meaning}}</div>

{{Word Audio}}
{{Sentence Audio}}
<br>
{{Picture}}

{{#Notes}}
	<br>
	<div style="font-size: 20px; padding-top:12px">Примітка: {{Notes}}</div>
{{/Notes}}

{{#Pitch Accent Notes}}
<div style="font-size: 20px; width: fit-content; max-width:40vw; margin: auto">
	<details><summary>Примітка до Інтонаційних Наголосів:</summary>
		<br>{{Pitch Accent Notes}}
	</details>
</div>
{{/Pitch Accent Notes}}

</div>
```

### Інші опції

Є кілька інших опцій.

#### Фурігана
Фурігана це читання канджі у хірагана написані над ними, якщо хочете вимкнути заберіть `furigana:`. Або можете скопіювати речення з фуріганою після перекладу, і забрати фурігану у верхньому реченні, щоб мати обидва.

#### Повна кастомізація карточки

Ви можете повністю змінити вигляд і вміст картки, ось `Шаблон передньої сторони` цієї колоди:

```CSS
<div lang="ja">
{{Word}}
<div style='font-size: 20px;'>{{Sentence}}</div>
</div>
```

Якщо ви хочете, наприклад лише карти з реченнями то заберіть `{{Word}}`. Не хочете речень спереду? Заберіть `<div style='font-size: 20px;'>{{Sentence}}</div>`. Хочете лише аудіо? Заберіть усе і додайте `{{Word Audio}}`, `{{Sentence Audio}}` чи обидва.

У вкладці `Стиль` є багато стильових опцій, це все CSS який можна змінити. Щоб взяти інший шрифт можна змінити `font-family`, для розмірів тексту `font-size`, і `text-align`, щоб розмістити текст, наприклад з початку рядка. Змінюйте `b{color: }`, щоб змінити колір виділених слів, наприклад `b{color: 'red'}` чи `b{color: #f6ff00}`, також можна забрати `b{color: }`, тощо. 

Детальніше в [документації Anki]{https://docs.ankiweb.net/templates/styling.html}. І звісно можна використовувати будь-який свій кастомний CSS.

</details>

## Трошки про колоду

Kaishi - 開始, що значить "початок". Це навіть не банально, я в шоці. Альтернативна канонічна назва цього перекладу крім KaishiUa це: <br/>
Yuashi - 湯足, що може значити "ванна для ніг".

## Помилки та пропозиції
Якщо знайшли якусь помилку, створіть пост на github issue трекері [ось тут](https://github.com/maksiksking/KaishiUa/issues). <br/>
В колоді є суржик, і так задумано. Крім того, пропущено кілька потрібних за правописом ком, бо вони лишні.

## Подяки
Це переклад [Kaishi 1.5k](https://github.com/donkuri/Kaishi), і вічна вдячність всім її авторам за таку чудову колоду.

- [Maksiks](https://github.com/maksiksking) - ручний переклад всіх слів, і речень, і приміток, і приміток до інтонаційних наголосів, і цієї сторінки, і скільки я вже випив чашок чаю, дайте поспати, рятуйте.
- Всі хто працювали над [оцим](https://shron1.chtyvo.org.ua/Bondarenko_Ivan/Yaponsko-ukrainskyi_slovnyk.pdf?) більш-менш нормальним словником, пригодився, щоб покращити доречність деяких перекладів.


