1. Составить список девайсов для тестирования мобильного приложения Velas Wallet на платформах Android/iOS.
Так, чтобы можно было успеть прогнать smoke тесты за 1 день. (Предположим, что прогон смоука на 1 девайсе занимает 30 минут).
Аргументировать свой выбор (ссылками/комментариями).

Будем предполагать, что основная аудитория, которая использует приложение Velas Wallet — это азиатский рынок, а также продукт используется во всем мире.

Поэтому в первую очередь стоит изучить статистику часто используемых девайсов по регионам для этого обратимся к ресурсу: https://gs.statcounter.com/vendor-market-share/mobile/  

Отфильтруем по региону Азия за последние 6 месяцев, и выделим самые используемые девайсы 
  Samsung (23, 62 %), Apple(17,24 %), Xiaomi(16,22 %) , Oppo ( 9,46 %), Vivo(8,4 %), Huawei(7,55 %)

Отфильтруем, по всему миру и выделим: Apple (29,39 %), Samsung (27,03 %), Xiaomi (10,89 %), Huawei( 7,46 %),Oppo(5,15 %), Vivo(4,15 %)

Так же, просмотрим сайты  https://www.browserstack.com/ , https://www.appbrain.com/ (для  Android) где размещена  статистика часто использованных  моделей девайсов и последних тенденций мирового ринка, но берем во внимание, что присутствуют модели которые были сняты с производства, поэтому  выбираем более новые.
И  сайт  https://developer.apple.com/ (для IOS) где размещена статистика использования IOS,
iPadOS

Проанализировав статистику   и совместимость приложение с операционными системами (подходят Android 5.0 и более новые версии; IOS 11,4 и более новые версии) выберем такие девайсы: 

Android
•	Samsung Galaxy A12 (11.0) 

•	Samsung Galaxy A21s (10.0)

•	Samsung Galaxy A50 (9.0)

•	Samsung Galaxy S9 Plus   (8.0)

•	Samsung Galaxy S7 (6.0)

•	Samsung Galaxy Tab S4(8.0) – tablet 

•	Xiaomi Redmi Note 8 (9.0)

•	Xiaomi Redmi 6A (8.0)

•	Oppo CPH1909 (10.0)

•	vivo Y11 (9.0)

•	Huawei P40 (10.0)

IOS

•	iPhone 8 Plus  (13.0)

•	Apple iPhone XR (12.0)

•	Apple iPad Air 2019 (13.0)

•	Apple iPhone 11 Pro (13.0)

•	Apple iPhone 11 (14.0)

Если мы предположим, что прогон смоука на 1 девайсе занимает 30 минут, а список девайсов составил из 16 штук, нам понадобиться 8 часов рабочего времени. 


2. Написать чек-лист на логин/регистрацию в веб приложение кошелька https://wallet.velas.com.

Для написания проверки использую вложенный чек-лист 

1)Проверка отображения на странице «language» иконок для выбора нужного языка

 2)Проверка выбора языка на странице
 
2.1) проверка на то что можно выбрать язык

2.2) проверка на что нельзя выбрать язык, где при наведении курсора значок «перечеркнутый круг»

3)Проверка отображения страницы для создания пароля, после выбора нужного языка 

4)Проверка кнопки «створити»

4.1) проверка отображения   страницы   для установки пароля

5)Проверка экранной клавиатуры

5.1) проверка экранной клавиатуры, при наведении на значок «клавиатура» в поле «Пароль» 

5.2) проверка заполнения поля «Пароль» с помощью экранной клавиатуры

5.3) проверка заполнения поля «Пароль» с помощью обычной клавиатуры ноутбука/компьютера 

5.4) проверка заполнения поля «Пароль» с помощью обычной клавиатуры ноутбука/компьютера и электронной 

6)Проверка заполнения поля «Пароль» валидными и невалидными значениями 

6.1) проверка заполнения поля допустимым и не допустимым количеством символов

6.2) проверка заполнения поля латиницей 

6.3) проверка заполнения поля цифровыми значениями 

6.4) проверка заполнения поля цифровыми значениями и латиницей 

6.5) проверка не заполнения поля «Пароль»

6.6) проверка ввода спецсимволов

7)Проверка скрытия пароля с помощью точек 

8)Проверка кнопки «встановити»

8.1) проверка отображения страницы Нова сід-фраза и 24 рандомных слова 

9)Проверка кнопки назад 

1)проверка возврата на страницу создания пароля

10)Проверка кнопки «скасувати»

10.1)проверка отображение предупреждающего уведомления, о том что будут скинуты все слова 

11)Проверка кнопки «Друк» 

11.1)проверка на то что файл для загрузки открывается на гугл диске


12)Проверка кнопки «далі» 

12.1)проверка отображения страницы  «Підтвердіть сід-фразу» с полем для ввода слова

12.2)проверка отображения  placeholder  в поле ввода «#1 слово» 

12.3)проверка заполнения поля словом,номер которого указан в placeholder

13)Проверка кнопки «далі» 

13.1)повтор заполнения поля словом 24 раза для формирование сід фрази

14)проверка заполнения поля "Пароль" невалидными значениями

14.1) проверка заполнения поля другими словами 

14.2) проверка заполнения поля спецсимволами 

14.3) проверка не заполнения поля 

14.4)проверка отображения предупреждающего уведомления, о том что слова не совпадают


15)проверка отображение страницы «Умови користування» и кнопкой «Підтвердити»

16)проверка кнопки «Підтвердити»

16.1) проверка отображения личного кабинета 

