Создаем нового пользователя с правами админа, генерируем ему пароль на 10 символов и сохраняем в кипере
Забираем права админа у пользовательcкой учетной записи
Установить правила [policy.zip](https://github.com/XarDok/admin_apm/files/6683913/policy.zip), взять их можно у Михаила Прозорова
Cбрасываем  пароль на учетке пользователь должен придумать новый а так же сменить название учетки
Меняем пароль в рут на yg4$He5DZm 
Настраиваем Iptables:
Запускаем скрипт [vpnlock.txt](https://github.com/XarDok/admin_apm/files/6683810/vpnlock.txt): 
 chmod +x vpnlock.sh
 ./vpnlock.sh
далее вводим команды:
 sudo apt-get install iptables-persistent
 dpkg-reconfigure iptables-persistent
 iptables-save > /etc/iptables/rules.v4
 ip6tables-save > /etc/iptables/rules.v6
 netfilter-persistent save
 netfilter-persistent start
Меняем имя хоста hostnamectl set-hostname nb-(фамилия пользователя)
