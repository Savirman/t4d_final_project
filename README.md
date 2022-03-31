<p>Требования к инфраструктуре:</p>
<ul>
<li>Сервера приложений: ubuntu 20.04&nbsp;[limit:webservers]</li>
<li>Сервер БД: ubuntu 20.04, DB MySQL&nbsp;[limit:mysql]</li>
<li>БН смотрит на 80 порт серверов приложений [limit:webservers]</li>
</ul>
<p>Ip-адреса серверов приложения:</p>
<p>wordpress [limit:webservers]</p>
<ul>
<li>5.188.142.6</li>
<li>185.241.192.50</li>
</ul>
<p>monitoring [limit:monitoring]</p>
<ul>
<li>89.208.85.81</li>
</ul>
<p>database [limit:mysql]</p>
<ul>
<li>87.239.109.35 //&nbsp;10.0.1.4</li>
<li>10.0.1.12</li>
</ul><br />Описание проекта:<br />Сервера приложений работают под управлением Apache HTTP server, свободно распространяемое ПО с открытым исходным кодом. Сервера баз данных под управлением MySQL. Мониторинг и система оповещения о сбоях основывается на связке двух, хорошо себя зарекомендовавших ПО &ndash; это Prometheus и Grafana. На серверах приложений установлена система управления содержимым, популярное и функциональное, свободно распространяемое ПО &ndash; WordPress.<br />На серверах приложений установлены базовые утилиты для работы в командной строке: tmux, htop, tree, mc, iotop.
<p>запуск playbook для группы серверов</p>
<p>ansible-playbook Playbook.yaml --limit <span>[name]</span></p>
grafana 11074 
nginx 2949 11280