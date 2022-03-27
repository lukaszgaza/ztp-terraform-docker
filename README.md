# Docker i Terraform

## Wprowadzenie

### Docker
Docker to narzędzie służące do konteneryzacji, czyli wirtualizacji na poziomie sytemu operacyjnego. Pozwala na tworzenie przenośnych i uniwersalnych kontenerów pozwalających na łatwą dystrybucję naszych aplikacji - kontenery mogą zawierać zarówno kod aplikacji jak i zainstalowane zależności (np. bazę danych) co ułatwia wdrażanie aplikacji.\
Docker jest dostępny na stronie [docker.com](https://www.docker.com/get-started/).\
Dobrym wprowadzenie do dockera można znaleźć [tutaj](https://docs.docker.com/get-started/).

### Terraform
Terraform to narzędzie do deklaratywnego opisywania infrastruktury do uruchamiania aplikacji. Pozwala zastąpić ręcznę konfigurację (ręczną modyfikację plików konfiguracyjnych czy "wyklikiwanie" konfiguracji) kodem. Dzięki temu konfiguracja jest bardziej odtwarzalna i może być przechowywana w repozytorium kodu. Terraform jest formą IaaC (Infrastructure as a Code).\
Terraform jest dostępny na stronie [terraform.io](https://www.terraform.io/downloads). Wprowadzenie do terraform jest dostępne [tutaj](https://learn.hashicorp.com/collections/terraform/docker-get-started).

## Zadania

1. Aplikacja w Javie uruchamiana w Dockerze (2 punkty)
   * aplikacja w nieskończonej pętli ma wypisywać na ekran `Java App is working`
   * aplikacja ma być uruchamiana w kontenerze
   * kod aplikacji oraz pliki konfiguracyjne (zarówno samej aplikacji jak i Dockera) mają znajdować się w katalogu `java-docker`
   * w pliku `java-docker/java-doc.md` należy umieścić instrukcje opisujące w jaki sposób należy uruchomic kontener z działającą aplikacją oraz w jaki sposób sprawdzić, że aplikacja działa
2. Aplikacja w Pythonie uruchomiona w Dockerze (2 punkty)
   * aplikacja w nieskończonej pętli ma wypisywać na ekran `Python App is working`
   * aplikacja ma być uruchamiana w kontenerze
   * kontener ma być tworzony za pomocą `terraform` - dokumentacja odpowiedniego providera znajduje się [tutaj](https://registry.terraform.io/providers/kreuzwerker/docker/latest/docs)
   * kod aplikacji oraz pliki konfiguracyjne (zarówno samej aplikacji jak i Dockera oraz terraform) mają znajdować się w katalogu `python-docker`
   * w pliku `python-docker/python-doc.md` należy umieścić instrukcje opisujące w jaki sposób należy uruchomic kontener z działającą aplikacją oraz w jaki sposób sprawdzić, że aplikacja działa