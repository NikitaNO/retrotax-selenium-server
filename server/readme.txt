1. «апуск хаба.
’аб будет принимать запросы от тестов и перенаправл€ть их к нужному узлу (с требуемой платформой/браузером).
ћожно настроить порт и другие параметры в hub_config.json.

-> java -jar selenium-server-standalone-2.47.1.jar -role hub -hubConfig hub_config.json

2. «апуск узла.
”зел - машина на которой будет непосредственно будут выполн€тьс€ тесты в браузерах.
ћожно запустить несколько узлов на разных платформах с разным набором браузеров.
¬ node_config.json можно настроить адрес хаба, к которому должен подключатьс€ узел и список браузеров, которые он поддерживает.
Ќа узле должны быть драйвера дл€ Chrome, IE, Opera. ѕути к ним об€зательно указать при запуске узла.

-> java -jar selenium-server-standalone-2.47.1.jar -role node -nodeConfig node_config.json -Dwebdriver.chrome.driver="C:\Selenium\drivers\chromedriver.exe" -Dwebdriver.ie.driver="C:\Selenium\drivers\IEDriverServer.exe" -Dwebdriver.opera.driver="C:\Selenium\drivers\operadriver.exe"
