1. ������ ����.
��� ����� ��������� ������� �� ������ � �������������� �� � ������� ���� (� ��������� ����������/���������).
����� ��������� ���� � ������ ��������� � hub_config.json.

-> java -jar selenium-server-standalone-2.47.1.jar -role hub -hubConfig hub_config.json

2. ������ ����.
���� - ������ �� ������� ����� ��������������� ����� ����������� ����� � ���������.
����� ��������� ��������� ����� �� ������ ���������� � ������ ������� ���������.
� node_config.json ����� ��������� ����� ����, � �������� ������ ������������ ���� � ������ ���������, ������� �� ������������.
�� ���� ������ ���� �������� ��� Chrome, IE, Opera. ���� � ��� ����������� ������� ��� ������� ����.

-> java -jar selenium-server-standalone-2.47.1.jar -role node -nodeConfig node_config.json -Dwebdriver.chrome.driver="C:\Selenium\drivers\chromedriver.exe" -Dwebdriver.ie.driver="C:\Selenium\drivers\IEDriverServer.exe" -Dwebdriver.opera.driver="C:\Selenium\drivers\operadriver.exe"
