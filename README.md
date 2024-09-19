## Скрипт для перевода pdf диагностик в excel  

**Задача**: оцифровка документов диагностики знаний обучающихся (МЦКО).  
На вход принимаются:  
* документы в формате `pdf`, содержание таблицы с результатами по заданиям, привязанным к шифрам диагностируемого  
* документы в формате `pdf`, содержание таблицы с соотнесением шифров с ФИО  

В *результате* работы **python**-скрипта: 
* отдельные excel-файлы результатов с ФИО  
* сводный excel-файл результатов с датами, предметами, ФИО, классами  

**! gitflick не отображает тетрадки Jupiter**. В тетрадке даны подробные разъяснения кода, для нормального отображения требуется её скачать.

В папке `files` лежат примеры исходных pdf-файлов с синтезированными данными, а также файл `pivot.xlsx` являющийся результатом выполнения скрипта. Также переменные `path`, `path_codes`, `path_results` и `path_to_extract` требуется определить таким образом, что есть корневая папка `path`, в которой находятся архивы с шифрами в `path/codes` (далее переменная `path_codes`) и `path/results` (далее переменная `path_results`) с шифрами и результатами диагностик соотвественно.
