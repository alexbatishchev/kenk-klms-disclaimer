# Помогаем Kaspersky Security 8 для Linux Mail Server говорить с пользователем на человеческом языке

## Настройка потока почты
* настраиваем KLMS на обработку почты согласно политике безопасности. Отмечаем теги, которыми он снабжает подозрительные письма

* создаем в Exchange правило(а) обработки почты, которое при обнаружении тега(ов) от KLMS в теме письма, добавляет предупреждение в тело письма (Prepend the disclaimer) 

## Обший шаблон текста предупреждения

```html
<h1><font color="red">ВНИМАНИЕ !!</font></h1>
<b>Антиспам-система предприятия распознала это письмо из внешней почты как подозрительное. </b><br>
Подобные письма могут содержать вредоносные вложения, ссылки на сайты злоумышленников, или заведомо ложную информацию. <br><br>
Будьте осторожны: 
<ul><li> Не открывайте ссылки и приложенные файлы
<li> Если письмо пришло от знакомого вам адресата, но содержит неожиданные сведения или запросы (ссылки на документы или сайты, приложенные файлы), уточните у отправителя по телефону или другим способом, действительно ли он отправлял вам это письмо. Помните что злоумышленники могли завладеть почтой вашего собеседника или подделать обратный адрес
<li>Не вводите пароли, телефоны, номера карт и другую персональную информацию, если по ссылкам из письма открываются сайты, которые их запрашивают, даже если сайты выглядят похоже на привычные (корпоративная или личная веб-почта, сайт предприятия, личный кабинет вашего банка и т.п.)
<li>Не доверяйте бездумно сведениям, содержащимся в письме. Злоумышленники могут сообщать вам что пароль истёк (и нужно его сообщить для замены), что на вашем компьютере работает троянская программа (и вы должны заплатить выкуп), что ваш отчёт в контролирующий орган не принят (и вам необходимо срочно ознакомиться с приложенной к письму претензией в формате PDF) и тому подобное. Помните, что злоумышленники стараются напугать жертву или заставить её торопиться, чтобы снизить осторожность.
</ul>

В случае малейших сомнений в подлинности сведений из письма, <b>свяжитесь со службой техподдержки предприятия по телефону 123-45. <br>
<hr>

```

## Автор
https://batishchev.ru/blog/kenk-klms-disclaimer
