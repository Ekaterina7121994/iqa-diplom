# Курсовой проект к модулю "Введение в тестирование"

## Правила выполнения курсового проекта

1. Объект тестирования: интернет-магазин https://henderson.ru. **Важно:** это реальный сайт, НЕ ТЕСТОВЫЙ, поэтому не надо совершать на нем покупки и прочие подобные действия.
1. Скопируйте шаблон таблицы на свой Google-диск [здесь](https://docs.google.com/spreadsheets/d/1Nl2_n46HvTIdv7JpbNLjOtMcWSuYpblZjyxlsBFKanY/edit?usp=sharing), укажите в названии файла свои фамилию, имя и группу вместо Name, Surname, Group. 
1. Проверьте настройки доступа в своем документе – чтобы в ваших гугл-документах и таблицах была открыта возможность комментировать всем пользователям в интернете, кому предоставлена ссылка.
1. В предоставленном шаблоне есть все шаблоны, которые нужны для выполнения задания.
1. В своей таблице прикрепляйте ссылки на выполненную работу по каждому заданию.
1. Вам необходимо выполнить 5 заданий, кроме задания со звездочкой (задание 3.2* и 2.2* выполняется по желанию).
1. Когда выполните все 5 заданий, прикрепите в личном кабинете ссылку на свою таблицу с решениями и ожидайте проверки преподавателя.
1. Курсовой проект считается принятым, когда все 5 заданий (кроме задания 3.2.* 2.2* по желанию) приняты преподавателем.
1. Если вам вернули ДЗ на доработку:
- Для заданий 1, 2.1, 3.1: доработанную версию надо создать в новом листе на изначальной таблице. Для этого мы [переименовываем](https://drive.google.com/file/d/1dGqZztwZjqlzu-4uyl170akGAfci59N7/view?usp=sharing) уже существующий лист в "ДЗ Версия 1", создаем новый через [дублирование](https://drive.google.com/file/d/1Ich_S9DlpeaQ0BBnalVf-Ip9grsOKESj/view?usp=sharing), новый лист переименовываем в "ДЗ Версия 2" и выполняем доработки уже в ней. Аналогично для доработок после второй. 
- Для остальных заданий добавляем новую информацию в старом файле или так, как будет согласовано с проверяющим преподавателем.
- Доработка по курсовому проекту отправляется студентом и проверяется преподавателем только после доработки всех пунктов, которые ее требуют.

## Задание 1

Написать чек-лист для функциональной проверки [личного кабинета зарегистированного авторизованного пользователя](https://henderson.ru/cabinet/) (включая функционал разделов) на сайте https://henderson.ru/.

**Требования к выполнению:**
* Чек-лист должен представлять собой структурированный (многоуровневый) список, который содержит набор функциональных позитивных и негативных проверок клиентской стороны компонентов объекта тестирования.
* При составлении списка проверок должны учитываться различные варианты состояний страниц. Например, при проверке функционала "Мои отзывы" мы проверяем не только состояние без отзывов, но и с ними.
* Мы ожидаем от вас список проверок функционала личного кабинета без учета хедера и футера страницы, то есть то, что есть в этой [области](https://drive.google.com/file/d/1rn6z04Erx7QjUmmTm4-R5MNNBgXpRSP2/view?usp=sharing).

## Задание 2

2.1. Необходимо написать набор тест-кейсов на проверку функционала восстановления пароля.

Ваша задача - написать минимум 20 тест-кейсов, которые должны покрывать все, что описано в требованиях по
[ссылке](https://docs.google.com/document/d/12deDbATIy0Xps8MiWvumNqHISfAlFc4etY8F4lPcqJ4/edit?usp=sharing), и учитывать позитивные и негативные кейсы.

2.2.*  Напишите свои вопросы по данным требованиям - они могут касаться не описанных, но важных сценариев, граничных значений и подобных проблем, по аналогии с ДЗ.

## Задание 3

3.1. На основе [скриншота](https://drive.google.com/file/d/1ucv3JFqEGY7ijVtP0Qn0BrdV2ipqYu37/view?usp=sharing) создать не менее трех баг репортов.

3.2* (необязательное задание). Найти баг в функционале "Написать отзыв" в карточке товара и составить на него баг-репорт. 
Если найдете несколько - замечательно!

## Задание 4

Вы тестируете страницу карточки товара. Из ТЗ вы знаете, что товар может стоить от 1 рубля до 10 000 000 рублей. К сожалению, на сайте в данный момент товаров с такой ценой нет, а разработчик бекенда в отпуске, поэтому вам нужно протестировать верстку страницы карточки товара с максимальной и минимальной ценой самостоятельно.
Ваша задача - самостоятельно определить, как проще это реализовать, и предоставить решение в виде скриншотов страницы (чтобы было видно, с помощью чего вы изменили эту цену) карточки товара с минимальной и максимальной ценой товара.

## Задание 5

Бекенд разработчик говорит, что мы отправляем данные с сайта в неправильном формате и просит вас помочь найти нужный запрос. Фронтенд разработчик ушел в отпуск в поход без связи, а документация пропала.

Известно, что проблема в данных, которые уходят в post запросе по адресу https://api.mindbox.ru/v3/js/operations/sync, и происходит это скорее всего при работе с личными данными пользователя (например авторизация, личный кабинет, просмотр корзины).

Ваша задача - изучить ответы и запросы при работе с сайтом; найти, как же выглядят параметры deviceUUID, requestId и status, и приложить скриншот искомого превью в таблицу с решениями.

### Как правильно задавать вопросы преподавателю?

Что поможет решить большинство частых проблем:

1. Попробовать найти ответ сначала самостоятельно в интернете или в материалах курса и только после этого спрашивать у преподавателя. Скилл поиска ответов пригодится вам в профессиональной деятельности.
1. Если вопросов больше одного, то присылайте их в виде нумерованного списка. Так преподавателю будет проще отвечать на каждый из них. 
1. При необходимости прикрепите к вопросу скриншоты и стрелочкой покажите, где не получается. 

Что может стать источником проблем:

1. Вопросы вида «Ничего не работает. Не запускается. Всё сломалось». Преподаватель не сможет ответить на такой вопрос без дополнительных уточнений. Цените своё время и время других.
2. Откладывание выполнения курсового проекта на последний момент.
3. Ожидание моментального ответа на свой вопрос. Преподаватели - работающие QA, которые занимаются, кроме преподавания, своими проектами. Их время ограничено, поэтому постарайтесь задавать правильные вопросы, чтобы получать быстрые ответы :)
