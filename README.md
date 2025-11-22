# Blue-Team---Network-Security-Final-Project
Network Security

International Network Security – Final Project

Projekt obejmował stworzenie pełnego środowiska sieciowego z wykorzystaniem pfSense, Kali Linux, Ubuntu, Debian oraz Windows, z naciskiem na bezpieczeństwo sieci, segmentację, kontrolę ruchu, testy komunikacji, firewalling oraz wdrożenie systemu IDS/IPS. Projekt odzwierciedla realne zadania wykonywane przez specjalistów Blue Team, Network Security oraz SOC.

1. Budowa i konfiguracja środowiska sieciowego

W ramach projektu skonfigurowano środowisko składające się z kilku różnych systemów operacyjnych podłączonych do dwóch podsieci zarządzanych przez pfSense. Każda maszyna otrzymała odpowiednią konfigurację adresów IP, zgodnie ze scenariuszem projektowym.

W środowisku uwzględniono:

-pfSense jako router i firewall,

-Kali Linux jako system testowy i ofensywny,

-Ubuntu i Debian jako serwery usług,

-Windows jako host użytkownika testującego połączenia.

2. Testowanie komunikacji i walidacja scenariusza

Przeprowadzono testy:

-łączności pomiędzy wszystkimi hostami,

-poprawności działania podsieci,

-dostępu między różnymi segmentami sieci,

-tras routingu oraz konfiguracji firewalli na pfSense.

-Weryfikacja potwierdziła, które połączenia działają, a które wymagają ręcznej konfiguracji (np. przekierowania portów, ustawienia firewall rules).

3. Konfiguracja systemów Ubuntu i Debian

Zrealizowano zadania obejmujące:

-konfigurację interfejsów sieciowych,

-analizę ruchu sieciowego,

-weryfikację usług,

-testy odpowiedzi na ping i połączenia TCP/UDP,

-przygotowanie serwerów do dalszej pracy w sieci testowej.

4. Project Task 1 – diagnostyka ruchu i konfiguracja usług

W tej części wykonano:

-konfigurację usług,

-analizę problemów z komunikacją,

-sprawdzenie poprawności działania usług sieciowych w poszczególnych systemach,

-testy dostępu między podsieciami,

-identyfikację błędów wynikających z błędnej konfiguracji lub braku tras.

5. Project Task 2 – NAT, firewall i dostęp do web servera

W ramach drugiego zadania:

-zidentyfikowano problem braku dostępu do web servera z hosta fizycznego,

-ustalono główną przyczynę: brak skonfigurowanego NAT na pfSense,

-wykonano konfigurację:

-NAT / Port Forwarding,

-firewall rules dla HTTP i SSH,

-ustawień umożliwiających dostęp do usług w sieci wewnętrznej.

Po konfiguracji usługi można było poprawnie osiągnąć z hosta fizycznego.

6. Testy usług HTTP i SSH

Przeprowadzono testy:

-działania serwera WWW,

-obsługi połączeń HTTP,

-połączeń SSH z różnych hostów,

-dostępu z sieci fizycznej przez pfSense.

Testy potwierdziły prawidłowość konfiguracji po wdrożeniu NAT i odpowiednich reguł firewall.

7. Project Task 3 – IDS/IPS (Suricata)

W tej części:

-wskazano Suricata jako odpowiednie rozwiązanie IDS/IPS spełniające wymagania CISO,

-rozpoczęto proces instalacji i konfiguracji,

-zidentyfikowano problem z aktualizacją pakietów Suricata (najprawdopodobniej błąd repozytoriów lub pfSense Package Manager), co uniemożliwiło wykonanie końcowych kroków.

-Mimo tego opisano plan konfiguracji i sposób działania systemu detekcji i zapobiegania włamaniom.

Efekt końcowy projektu

Projekt dostarczył:

-kompletne środowisko sieciowe z wieloma systemami operacyjnymi,

-poprawnie działający routing i NAT,

-skonfigurowane reguły firewall,

-przetestowane usługi SSH i HTTP,

-analizę oraz diagnostykę problemów komunikacyjnych,

-przygotowanie architektury sieciowej pod system IDS/IPS,

-symulację prawdziwego środowiska bezpieczeństwa sieciowego.

To praktyczne doświadczenie pokazuje umiejętność pracy z pfSense, segmentacją sieci, firewallami, NAT-em, protokołami sieciowymi oraz usługami serwerowymi — kompetencje kluczowe w pracy Blue Team / SOC / Network Security.
