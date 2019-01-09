# PLV8 2.3.8 для Postgresql 11, ubuntu 18 x64.
## PLV8-Postgresql11-Ubuntu-18
Должен быть установлен libc++-dev 
```
sudo apt-get install libc++-dev
```
Содержимое каталога переносим в папку usr,
если из командной строки то переключаемся на пользователя postgres 

```
sudo su - postgres
```
входим в psql
```
psql
```
И создаём расширение
```
CREATE EXTENSION plv8;
```
Проверяем
```
SELECT plv8_version();
  plv8_version
-----------------
2.3.8
(1 row)
```
пользуемся

@@thnaks I have followed the same thing. but I am facing issues help me 
ERROR:  could not load library "/usr/lib/postgresql/11/lib/plv8-2.3.8.so": libc++abi.so.1: cannot open shared object file: No such file or directory
