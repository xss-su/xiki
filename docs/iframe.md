# Ифрэйм 
Ифрэйм, iframe - это два понятия объединенные одним словом. 

## Iframe код 

Это способ управления трафиком, а вернее - способом его отправки на нужный нам адрес. Данный способ заключается в вставке в страницу сайта специально сгенерированного кода, который незаметно от пользователя подгружает в фоновом режиме нашу страницу. Такой трафик используется как для связок так и для накрутки посещаемости сайтов и др. 
Метод довольно прост. В тело сайта вставляется код вида 
```html
<iframe src='http://site.com' style='visibility:none'></iframe> 
```

Такой код и выполнит незаметный для пользователя фоновый переход на сайт site.com. 
(См. Крипт)[crypt.md]

## Iframe процесс 

Это сам процесс внедрения нашего iframe кода на страницы сайта. Он бывает ручным и автоматическим. 
Ручной - это когда пользователь сам заходит по ftp или через шелл на сайт и размещает в зависимости от ситуации код на сайте. 
Автоматический - это процесс использующий программные средства. Такие программы называются фрэймерами (ифрэймер), которые работают в автоматическом режиме и сами размещают код на сайтах. Естественно, что ифрэймер обрабатывает намного больше сайтов за единицу времени. Но эти продукты имеют и недостатки. К ним можно отнести "тупость". т.е. программы зачастую вставляют код во все доступные (html и php) файлы не делая выбор где нужно, а где нет. Такой процесс может сделать сайт неработоспособным. "Умные" фрэймеры делают процесс более результативным. Они анализируют файл перед вставкой кода и решают нужно ли вставлять код или нет. Такие продукты несколько дороже. Пример: Ziframer (для *nix систем) и FTP_admin (для win систем).
