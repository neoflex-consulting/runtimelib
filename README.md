# runtimelib
Library collection for standalone Datagram installation 

Для получения набора библиотек выполнить _mvn -U -Pspark2 clean dependency:copy-dependencies_, после чего набор появится в target/sparklib

# maven offline repository
В среде исполнения зачастую нет доступа к ресурсам интернет, а для сборки трансформаций и прочих артефактов Datagram требуется репозиторий с набором библиотек. 

Для сборки такого репозитория предлагается выполнить команду\
`mvn -f m2.xml -Pspark2 package -Dmaven.repo.local=./repository` 
указав нужный профиль -Pspark2 или -Pspark3
