# UiPath

Automatyzacja RPA (Robotic Process Automation) to technologia, która wykorzystuje roboty programowe (tzw. boty) do automatyzacji powtarzalnych, regulowanych zadań wykonywanych na komputerze. Roboty te naśladują działania człowieka w różnych aplikacjach i systemach, wykonując takie czynności jak:

* **Wprowadzanie danych:** Wypełnianie formularzy, wprowadzanie danych do systemów.
* **Przetwarzanie danych:** Kopiowanie, przenoszenie, sortowanie, filtrowanie danych.
* **Integracja systemów:** Łączenie różnych aplikacji i systemów, przesyłanie danych między nimi.
* **Generowanie raportów:** Tworzenie raportów na podstawie danych z różnych źródeł.
* **Obsługa poczty elektronicznej:** Odczytywanie, wysyłanie, sortowanie wiadomości e-mail.

**Jak działa automatyzacja RPA?**

Roboty RPA działają na poziomie interfejsu użytkownika, czyli tak samo jak człowiek, klikając w przyciski, wpisując tekst, czy otwierając pliki. Dzięki temu nie trzeba wprowadzać zmian w istniejących systemach, co znacznie ułatwia i przyspiesza wdrożenie automatyzacji.

**Korzyści z automatyzacji RPA:**

* **Zwiększenie wydajności:** Roboty pracują szybciej i dokładniej niż ludzie, co pozwala na zwiększenie wydajności procesów.
* **Redukcja kosztów:** Automatyzacja pozwala na ograniczenie kosztów pracy, eliminując potrzebę ręcznego wykonywania zadań.
* **Poprawa jakości:** Roboty nie popełniają błędów wynikających z czynnika ludzkiego, co przekłada się na poprawę jakości danych i procesów.
* **Zwiększenie elastyczności:** Roboty mogą być łatwo dostosowywane do zmieniających się potrzeb biznesowych.
* **Poprawa satysfakcji pracowników:** Automatyzacja pozwala odciążyć pracowników od monotonnych, powtarzalnych zadań, umożliwiając im skupienie się na bardziej wartościowych i kreatywnych czynnościach.

**Gdzie można zastosować automatyzację RPA?**

Automatyzacja RPA znajduje zastosowanie w wielu branżach, m.in.:

* **Finanse i księgowość:** Przetwarzanie faktur, księgowanie, raportowanie.
* **Obsługa klienta:** Obsługa zgłoszeń, udzielanie odpowiedzi na pytania.
* **Zasoby ludzkie:** Obsługa procesów kadrowych, naliczanie wynagrodzeń.
* **Logistyka:** Zarządzanie zamówieniami, śledzenie przesyłek.
* **Administracja:** Obsługa dokumentów, wprowadzanie danych.

**UiPath a automatyzacja RPA**

UiPath to jedna z wiodących platform do automatyzacji RPA, która oferuje szeroki zakres narzędzi i funkcjonalności do tworzenia, wdrażania i zarządzania robotami. Dzięki intuicyjnemu interfejsowi graficznemu i bogatej bibliotece aktywności, UiPath umożliwia tworzenie robotów nawet osobom bez doświadczenia w programowaniu.

Dokładniejsze spojrzenie na każdy podstawowy element:

**UiPath Studio** to zintegrowane środowisko programistyczne (IDE), w którym programiści automatyzacji projektują, tworzą i debuggują projekty automatyzacji. Studio można połączyć z Orchestratorem, co ułatwia publikowanie projektów automatyzacji jako pakiety NuGet za pośrednictwem dedykowanych kanałów. Stamtąd są one dystrybuowane do robotów w celu wykonania.

Mówiąc o Studio, możemy myśleć o dwóch profilach, a mianowicie Studio i StudioX. Są one przeznaczone dla różnych umiejętności programistycznych, jakie mogą posiadać twórcy:

* **StudioX** jest przeznaczone dla użytkowników biznesowych, którzy chcą zautomatyzować zadania dla siebie i swoich najbliższych zespołów.
* **Studio** jest przeznaczone dla programistów automatyzacji, którzy chcą tworzyć złożone nienadzorowane lub nadzorowane automatyzacje procesów.

W zależności od rodzaju licencji Studio zakupionej przez przedsiębiorstwo, użytkownicy Studio mogą przełączać się między profilami Studio i StudioX w zależności od potrzeb.

**Robot** to agent wykonawczy, który uruchamia automatyzacje zbudowane za pomocą rodziny Studio, a następnie opublikowane jako pakiety lokalnie lub w Orchestratorze.

Istnieją dwa rodzaje robotów UiPath i różnią się one zarówno sposobem działania, jak i licencjonowaniem:

* **Roboty nadzorowane (Attended)**:
    * Są cyfrowymi pomocnikami dla użytkowników. Działają na tych samych komputerach co ludzie, w tych samych godzinach.
    * Są uruchamiane bezpośrednio przez ludzi (zwykle za pośrednictwem UiPath Assistant) lub przez zdarzenie związane z tym, co robi użytkownik, np. otwarcie aplikacji lub otrzymanie wiadomości e-mail.
    * **UiPath Assistant** to komponent, który zapewnia przyjazny interfejs do interakcji z robotami nadzorowanymi. Jest to narzędzie, którego używamy do łatwego dostępu, zarządzania i uruchamiania automatyzacji.
* **Roboty nienadzorowane (Unattended)**:
    * Są przeznaczone do pracy bez przerwy, z minimalnym udziałem użytkowników.
    * Są wdrażane na oddzielnych maszynach, a ich zadania są uruchamiane wyłącznie z Orchestratora.
    * Ich interakcje z użytkownikami są zazwyczaj obsługiwane z jak najmniejszym zakłóceniem, poprzez tworzenie i wysyłanie żądań o dane wejściowe lub walidację jako zadania.
    * Podczas oczekiwania na przetworzenie danych wejściowych, roboty nienadzorowane mogą kontynuować swoją pracę, podejmując inne zadania.
    * Gdy dane wejściowe zostaną dostarczone, roboty nienadzorowane mogą wznowić pracę nad procesem.

* **Roboty chmurowe (Automation Cloud Robots - ACR)**:
    * To roboty SaaS hostowane w UiPath Automation Cloud, które umożliwiają szybkie uruchamianie automatyzacji bez konieczności budowania lub zarządzania własną infrastrukturą robota nienadzorowanego.
    * Występują w dwóch wersjach:
        * **VM Automation Cloud Robots:** Dostęp do w pełni konfigurowalnej wirtualnej maszyny Windows i konfiguracja robotów UiPath do uruchamiania dowolnego zadania w ciągu kilku minut.
        * **Serverless Automation Cloud Robots:** Uruchom projekty w tle, na wielu platformach, bez martwienia się o konfigurację infrastruktury. Możesz więc udostępniać, zarządzać i skalować te roboty z Automation Cloud. Innymi słowy, UiPath zajmuje się wszystkim - infrastrukturą i robotami.
* **Roboty testowe (Test Robots)**:
    * Roboty te mogą być wdrażane w celu wykonywania testów na żądanie, w sposób ciągły i na dużą skalę.
    * Oto niektóre z cech robota testowego:
        * Zbudowane specjalnie do testowania przepływów pracy, aktywności i aplikacji.
        * Zapewniają elastyczność w zarządzaniu i ponownym wykorzystywaniu przypadków testowych w różnych projektach.
        * Umożliwiają testowanie jednostkowe na poziomie aktywności od razu po wyjęciu z pudełka.


**Orchestrator**, serce zarządzania automatyzacją, to aplikacja internetowa, która umożliwia zarządzanie, kontrolowanie i monitorowanie robotów i automatyzacji. Za pomocą Orchestratora możemy wdrażać, uruchamiać, mierzyć, udostępniać, śledzić i zapewniać bezpieczeństwo każdego robota w organizacji.

Orchestrator działa również jako repozytorium bibliotek, komponentów wielokrotnego użytku, zasobów i procesów używanych przez roboty lub programistów.

Główne możliwości Orchestratora to:

* **Udostępnianie:** tworzy i utrzymuje połączenie z robotami.
* **Kontrola i dystrybucja licencji:** umożliwia tworzenie, przypisywanie i utrzymywanie licencji, ról, uprawnień, grup i hierarchii folderów.
* **Przechowywanie i dystrybucja automatyzacji:** umożliwia kontrolowane przechowywanie i dystrybucję projektów automatyzacji, zasobów i poświadczeń, a także dużych plików używanych w automatyzacjach.
* **Uruchamianie zadań automatyzacji w trybie nienadzorowanym:** umożliwia tworzenie i dystrybucję zadań automatyzacji na różne sposoby, w tym za pomocą kolejek i wyzwalaczy.
* **Monitorowanie:** umożliwia monitorowanie zadań i robotów oraz przechowuje dzienniki do celów audytu i analizy.
