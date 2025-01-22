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
conda install conda-forge::requests conda-forge::xlwings conda-forge::openpyxl conda-forge::pandas conda-forge::mysql-connector-python conda-forge::exchangelib
```

- Jeżeli instalacja modułów zakończy się sukcesem, konfiuguracja proxy nie będzie potrzebna.
- Instalacja powinna przebiegać mniej więcej jak na dołączonym poniżej logu.

```
(base) C:\Users\tacia>conda install conda-forge::requests conda-forge::xlwings conda-forge::openpyxl conda-forge::pandas conda-forge::mysql-connector-python conda-forge::exchangelib
Channels:
 - defaults
 - conda-forge
Platform: win-64
Collecting package metadata (repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: C:\Users\tacia\anaconda3\envs\test

  added / updated specs:
    - conda-forge::exchangelib
    - conda-forge::mysql-connector-python
    - conda-forge::openpyxl
    - conda-forge::pandas
    - conda-forge::requests
    - conda-forge::xlwings


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    blinker-1.9.0              |  py312haa95532_0          24 KB
    cryptography-43.0.3        |  py312hbd6ee87_1         1.3 MB
    libexpat-2.6.4             |       he0c23c2_0         136 KB  conda-forge
    libiconv-1.17              |       hcfcfb64_2         621 KB  conda-forge
    liblzma-5.6.3              |       h2466b09_1         102 KB  conda-forge
    libxml2-2.10.4             |       hc3477c8_0         1.7 MB  conda-forge
    libxslt-1.1.37             |       h2bbff1b_1         447 KB
    libzlib-1.3.1              |       h2466b09_2          54 KB  conda-forge
    lxml-5.2.1                 |  py312h09808a7_0         1.1 MB
    mysql-common-9.0.1         |       h2224204_4         631 KB  conda-forge
    mysql-connector-python-9.0.0|  py312h275cf98_1         505 KB  conda-forge
    mysql-libs-9.0.1           |       h809f9c2_4         1.2 MB  conda-forge
    pyjwt-2.10.1               |  py312haa95532_0          87 KB
    python-3.12.8              |h3f84c4b_1_cpython        15.1 MB  conda-forge
    tk-8.6.13                  |       h5226925_1         3.3 MB  conda-forge
    zlib-1.3.1                 |       h2466b09_2         105 KB  conda-forge
    zstd-1.5.6                 |       h0ea2cb4_0         341 KB  conda-forge
    ------------------------------------------------------------
                                           Total:        26.8 MB

The following NEW packages will be INSTALLED:

  blas               pkgs/main/win-64::blas-1.0-mkl
  blinker            pkgs/main/win-64::blinker-1.9.0-py312haa95532_0
  brotli-python      pkgs/main/win-64::brotli-python-1.0.9-py312h5da7b33_9
  cached-property    pkgs/main/noarch::cached-property-1.5.2-py_0
  certifi            pkgs/main/win-64::certifi-2024.12.14-py312haa95532_0
  cffi               pkgs/main/win-64::cffi-1.17.1-py312h827c3e9_1
  charset-normalizer pkgs/main/noarch::charset-normalizer-3.3.2-pyhd3eb1b0_0
  cryptography       pkgs/main/win-64::cryptography-43.0.3-py312hbd6ee87_1
  defusedxml         pkgs/main/noarch::defusedxml-0.7.1-pyhd3eb1b0_0
  dnspython          pkgs/main/win-64::dnspython-2.4.2-py312haa95532_0
  et_xmlfile         pkgs/main/win-64::et_xmlfile-1.1.0-py312haa95532_1
  exchangelib        conda-forge/win-64::exchangelib-5.5.0-py312h2e8e312_0
  idna               pkgs/main/win-64::idna-3.7-py312haa95532_0
  intel-openmp       pkgs/main/win-64::intel-openmp-2023.1.0-h59b6b97_46320
  isodate            pkgs/main/win-64::isodate-0.6.1-py312haa95532_0
  libexpat           conda-forge/win-64::libexpat-2.6.4-he0c23c2_0
  libiconv           conda-forge/win-64::libiconv-1.17-hcfcfb64_2
  liblzma            conda-forge/win-64::liblzma-5.6.3-h2466b09_1
  libsqlite          conda-forge/win-64::libsqlite-3.48.0-h67fdade_0
  libxml2            conda-forge/win-64::libxml2-2.10.4-hc3477c8_0
  libxslt            pkgs/main/win-64::libxslt-1.1.37-h2bbff1b_1
  libzlib            conda-forge/win-64::libzlib-1.3.1-h2466b09_2
  lxml               pkgs/main/win-64::lxml-5.2.1-py312h09808a7_0
  mkl                pkgs/main/win-64::mkl-2023.1.0-h6b88ed4_46358
  mkl-service        pkgs/main/win-64::mkl-service-2.4.0-py312h827c3e9_2
  mkl_fft            pkgs/main/win-64::mkl_fft-1.3.11-py312h827c3e9_0
  mkl_random         pkgs/main/win-64::mkl_random-1.2.8-py312h0158946_0
  mysql-common       conda-forge/win-64::mysql-common-9.0.1-h2224204_4
  mysql-connector-p~ conda-forge/win-64::mysql-connector-python-9.0.0-py312h275cf98_1
  mysql-libs         conda-forge/win-64::mysql-libs-9.0.1-h809f9c2_4
  ntlm-auth          pkgs/main/noarch::ntlm-auth-1.5.0-pyhd3eb1b0_0
  numpy              pkgs/main/win-64::numpy-2.0.1-py312hfd52020_1
  numpy-base         pkgs/main/win-64::numpy-base-2.0.1-py312h4dde369_1
  oauthlib           pkgs/main/win-64::oauthlib-3.2.2-py312haa95532_0
  openpyxl           conda-forge/win-64::openpyxl-3.1.5-py312he70551f_1
  pandas             conda-forge/win-64::pandas-2.2.3-py312h72972c8_1
  pycparser          pkgs/main/noarch::pycparser-2.21-pyhd3eb1b0_0
  pygments           pkgs/main/win-64::pygments-2.15.1-py312haa95532_1
  pyjwt              pkgs/main/win-64::pyjwt-2.10.1-py312haa95532_0
  pysocks            pkgs/main/win-64::pysocks-1.7.1-py312haa95532_0
  python-dateutil    pkgs/main/win-64::python-dateutil-2.9.0post0-py312haa95532_2
  python-tzdata      pkgs/main/noarch::python-tzdata-2023.3-pyhd3eb1b0_0
  python_abi         conda-forge/win-64::python_abi-3.12-5_cp312
  pytz               pkgs/main/win-64::pytz-2024.1-py312haa95532_0
  pywin32            pkgs/main/win-64::pywin32-308-py312h5da7b33_0
  requests           conda-forge/noarch::requests-2.32.3-pyhd8ed1ab_1
  requests-negotiat~ conda-forge/win-64::requests-negotiate-sspi-0.5.3-py312h2e8e312_3
  requests-oauthlib  pkgs/main/win-64::requests-oauthlib-2.0.0-py312haa95532_0
  requests_ntlm      pkgs/main/noarch::requests_ntlm-1.1.0-pyhd3eb1b0_0
  six                pkgs/main/noarch::six-1.16.0-pyhd3eb1b0_1
  tbb                pkgs/main/win-64::tbb-2021.8.0-h59b6b97_0
  tzlocal            pkgs/main/win-64::tzlocal-5.2-py312haa95532_0
  ucrt               pkgs/main/win-64::ucrt-10.0.20348.0-haa95532_0
  urllib3            pkgs/main/win-64::urllib3-2.3.0-py312haa95532_0
  vc14_runtime       conda-forge/win-64::vc14_runtime-14.42.34433-he29a5d6_23
  win_inet_pton      pkgs/main/win-64::win_inet_pton-1.1.0-py312haa95532_0
  xlwings            conda-forge/win-64::xlwings-0.33.6-py312h2e8e312_0
  zstd               conda-forge/win-64::zstd-1.5.6-h0ea2cb4_0

The following packages will be UPDATED:

  openssl              pkgs/main::openssl-3.0.15-h827c3e9_0 --> conda-forge::openssl-3.4.0-ha4e3fda_1
  python                pkgs/main::python-3.12.8-h14ffc60_0 --> conda-forge::python-3.12.8-h3f84c4b_1_cpython
  vs2015_runtime     pkgs/main::vs2015_runtime-14.42.34433~ --> conda-forge::vs2015_runtime-14.42.34433-hdffcdeb_23
  zlib                    pkgs/main::zlib-1.2.13-h8cc25b3_1 --> conda-forge::zlib-1.3.1-h2466b09_2

The following packages will be SUPERSEDED by a higher-priority channel:

  tk                        pkgs/main::tk-8.6.14-h0416ee5_0 --> conda-forge::tk-8.6.13-h5226925_1


Proceed ([y]/n)? y


Downloading and Extracting Packages:

Preparing transaction: done
Verifying transaction: done
Executing transaction: done

(base) C:\Users\tacia>
```

3. **Konfiguracja proxy**

- Jeżeli pojawią się problemy z pobranienm modułów, konieczne może być dokonfigurowanie ustawień proxy.

```yaml
proxy_servers:
    http: http://username:password@corp.com:8080
    https: https://username:password@corp.com:8080
```

- https://docs.anaconda.com/working-with-conda/reference/proxy/
- https://docs.conda.io/projects/conda/en/latest/user-guide/configuration/settings.html#proxy-servers-configure-conda-for-use-behind-a-proxy-server
- 


4. **Dodatkowe certyfikaty**
- Jeżeli 
