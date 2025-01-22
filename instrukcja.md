# Instrukcja przygotowania i weryfikacji środowiska

1. **Instalacja środowiska**
- Proszę pobrać instalator z oficjalnej strony [Anaconda](https://www.anaconda.com/products/distribution#download-section)
- Następnie przeprowadzić instalację. Instalator jest dość typowy. Środowisko można zainstalować dla bieżącego użytkownika, nie ma potrzeby przeprowadzania instalacji dla wszystkich użytkowników systemu.
- Szczegółowa instrukcja instalacji znajduje się w dokumentacji: [Installing Anaconda Distribution](https://docs.anaconda.com/anaconda/install/)

2. **Uruchomienie i weryfikacja**
- Po zakończonej instalacji proszę uruchomić **Anaconda Navigator**, przejść do zakładki **Environments**, kliknąć w zielony przycisk i z menu wybrać **Terminal**

![image](./step-1.png)

- W uruchomionym terminalu, musi być widoczna nazwa uruchomionego środowiska:

![image](./step-2.png)

- Następnie proszę przeprowadzić instalację modułów z których będziemy korzystać w trakcie szkolenia. Wystarczy uruchomić poniższe polecenie:

```
conda install requests xlwings openpyxl pandas mysql-connector-python exchangelib
```

4. **Konfiguracja proxy**
