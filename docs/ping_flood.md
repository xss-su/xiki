# Ping-флуд 
Ping-flood, дословно: наводнение пакетами ping — тип атаки на сетевое оборудование, ставящий своей целью отказ в обслуживании. Ключевой особенностью (по сравнению с остальными видами флуд-атак) является возможность осуществления атаки «бытовыми средствами» (программами и утилитами, входящими в состав домашних/офисных версий операционных систем).

## Суть атаки 
ICMP-сообщение (эхо-запрос) обрабатывается сетевым оборудованием третьего (и выше) уровня. В большинстве случаев это оборудование использует программные средства маршрутизации и обработки пакетов. При этом эхо-запрос требует от устройства принятия пакета, его обработки и формирования/отправки пакета с ответом на запрос. Объём выполняемых действий при этом многократно превышает объём работы по маршрутизации обычного пакета. Размер ICMP-запроса обычно небольшой (около 64 байт, при максимальном размере пакета IP 64 кбайт). В результате, при формальном сохранении небольшого трафика, возникает перегрузка по количеству пакетов, и устройство начинает пропускать остальные пакеты (по другим интерфейсам или протоколам), что и является целью атаки. 

## Ограничения ICMP флуда 
Некоторые провайдеры в договоре оговаривают отдельным пунктом ограничение на скорость ICMP-пакетов, оставляя за собой право прекращения предоставления услуги в случае ICMP флуда, нарушающего работу сетевого оборудования. 

## Распределённая атака 

При распределённой атаке (с нескольких тысяч узлов), ICMP-запросы поступают с обычной скоростью тестирования (около 1 пакета в секунду с узла), но одновременно с нескольких тысяч компьютеров. В этом случае итоговая нагрузка на устройство, являющееся целью атаки, может достигать пропускной способности канала (и заведомо превосходить скорость обработки пакетов устройством). 
В апреле 2007 года сайты правительства Эстонии подверглись распределённой ICMP-атаке. В качестве «орудия» атаки использовалась диагностическая утилита ping, отправляющая пакет объёмом 20000 байт на сайт www.riik.ee. По сообщениям СМИ атака была успешной.
> Хакеры атакуют эстонские правительственные сайты — lenta.ru.

В 2010 году мощность одной распределённой DDoS-атаки впервые превысила 100 ГБит/сек. 

## Противодействие атаке 
Для противодействия атаке (помимо блокирования трафика с отдельных узлов и сетей) возможны следующие меры: 
 - Отключение ответов на ICMP-запросы (отключение соответствующих служб или предотвращение отклика на определенный тип сообщения) на целевой системе; 
 - Понижение приоритета обработки ICMP-сообщений (при этом весь остальной трафик обрабатывается в обычном порядке, а ICMP-запросы обрабатываются по остаточному принципу, в случае перегрузки ICMP-сообщениями часть из них игнорируется). 
 - Отбрасывание или фильтрация ICMP-трафика средствами межсетевого экрана (фаервола). 
 - Увеличение очереди обрабатываемых подключений.
