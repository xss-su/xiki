# Крипт 
Крипт, crypt - процесс сокрытия вашего вредоносного кода от антивирусов (далее по тексту АВ). 
К процессу крипта относят три основных понятия: 
 - Крипт exe файлов 
 - Крипт сплоитов/связок 
 - Крипт (или псевдо-крипт) iframe кода 

# Крипт exe 

Это процесс модификации кода вашего файла (exe/dll) таким образом, при котором сохранится работоспособность самого файла и при этом все антивирусы будут считать что файл безвредный для системы. Это достигается различными способами. Самые простые - это добавление в код файла мусорных секция или ложных вызовов и прыжков. Такой простейший способ давно потерял свою актуальность ввиду развития антивирусов и логистических способов анализа файла (эвристический анализ). 
Сейчас применяются более сложные способы которые включают в себя огромный комплекс модификаций файшего файла. И чем изощереннее способы тем дольше ваш файл будет оставаться "чистым" для АВ. 
Такой крипт бывает двух видов: 
 - Ручной - это когда ваш файл модифицируется ручным способом индивидуально под задачу. Считается, что такой способ дает более качественный результат и файл дольше остается "чистым". 
 - При помощи криптора - это автоматический способ при котором заранее написана программа, которая и производит ряд стандартных для каждого файла модификаций. Такой способ считается менее надежным т.к. процедуры производимые над файлом одинаковы для всех файлов. Что в свою очередь значит, что если один из файлов попался на "улов" к АВ то и все остальные в ближайшее время начнут детектиться (определяться АВ как вредоносные). 
При каждой такой модификации (процессе) размер файла увеличивается на определенное количество килобайт. Этот размер у каждого сервиса/криптора разный и может варьироваться от 5кб до 300кб. Чем меньше - тем лучше. Добавочный размер называется СТАБ-ом. Цена варьируется в пределах 5 - 50$. Автоматический (при помощи криптера стоит 5-15$), ручной стоит 25-50$. 

# Крипт сплоитов/связок 
Это процесс модернизации эксплоитов в cвязке до отсутствия срабатывания АВ. Принцип во многом схож с обычным криптом, но и при этом значительно отличается т.к. приходится работать сразу с несколькими языками программирования и модификаторами. Такой крипт значительно сложнее и очень редко происходит в автоматическом режиме. Сплоиты постоянно меняются и каждый раз приходится придумывать новые способы. Стоимость варьируется в пределах 20-100$ в зависимости от сложности работы. 

#Крипт Iframe 
Это процесс обфускации (изменения iframe кода) до состояния отсутствия реакции АВ. Зачастую связан с сложными модификациями на языке JavaScript. Стоит в пределах 5-15$. Часто автоматический.