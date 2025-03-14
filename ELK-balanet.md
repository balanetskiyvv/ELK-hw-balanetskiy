### Задание 1. Elasticsearch 

Установите и запустите Elasticsearch, после чего поменяйте параметр cluster_name на случайный.  

<img width="603" alt="изображение" src="https://github.com/user-attachments/assets/0d1df727-3be9-49e0-9a7c-233c7db47291" />

---

### Задание 2. Kibana

Установите и запустите Kibana.  

<img width="717" alt="изображение" src="https://github.com/user-attachments/assets/2957d4bb-5d8c-4ad1-93ed-894d15edb589" />

---

### Задание 3. Logstash

Установите и запустите Logstash и Nginx. С помощью Logstash отправьте access-лог Nginx в Elasticsearch.  
Успех был достигнут благодаря 2 суткам тяжелых поисков, чтобы понять как чуток конфиг logstash к нюансам, а именно 1 строка в output -> ssl_sertificate_verification 

<img width="1677" alt="изображение" src="https://github.com/user-attachments/assets/581f9db3-f377-4fc7-a76a-0f539730707b" />

P.S. А также синтаксис и кавычки (делалось на отдельных ВМ для проверки):  
<img width="449" alt="изображение" src="https://github.com/user-attachments/assets/70258da3-eabe-4607-b092-5b8e54e97046" />

---

### Задание 4. Filebeat. 

Установите и запустите Filebeat. Переключите поставку логов Nginx с Logstash на Filebeat.  

В docker-composer не удалось провернуть, поднял две ВМ в Яндекс.Облако и настроил вручную.  



---

### Задание 5*. Доставка данных 

Настройте поставку лога в Elasticsearch через Logstash и Filebeat любого другого сервиса , но не Nginx. 
Для этого лог должен писаться на файловую систему, Logstash должен корректно его распарсить и разложить на поля. 

*Приведите скриншот интерфейса Kibana, на котором будет виден этот лог и напишите лог какого приложения отправляется.*
