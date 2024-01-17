whoami
ls
cd
rm
rv
cp
touch
mkdir
rmdir
sudo
ls
grep np:  
ls -la | grep nazwa_katalogu
grep 'tekst' nazwa_pliku.txt
grep -r 'tekst' nazwa_katalogu
grep -i 'tekst' - wyszukuje po 'tekst'
grep -n - pokazuje numery wierszy
grep -l "tekst" *.txt - szuka te pliki co zawierają 'tekst'
grep -v "tekst" *.txt - szuka te pliki co NIE zawierają 'tekst'
find nazwa_pliku
find /nazwa_katalogu
find /path -perm 644
find /path -size +10M
find /path -mtime 10

> - nadpisanie i utworzenie pliku
>> - dodanie
< - wsad do polecenia
| - pipe - w jednym wierszu możemy wrzucic wiele poleceń kiedy tym oddzielimy

ping [ip]
ping oonet.pl -t
ping onet.pl -s 1M

ssh user@ip
sshkeygen
ssh-copy-id iser@ip

scp (Secure copy)
scp lokalny_katalog user@ip:[zdalny_katalog]
scp -r -p lokalny_katalog user@ip:[zdalny_katalog] -r cały katalog z podkatalogami -p metadane

rysnc - synchroniczne kopiowanie

procesy
ps - aktywne procesy

ps aux
ps aux | grep nazwa

top - interaktywne monitorowanie procesów
htop - jak top ale mocniejszy temat

kill [PID]
kill [nazwa_procesu]
kill all

df - disk free 
df -h
du - disk useage
du -sh

free -h

curl, wget - pobieranie danych
tar, zip, unzip - kompresja i dekompresja danych

sieciowe

netstat - informacje o polaczeniach
netstat -r --routing
netstat -i --interface
netstat -tuln

ipconfig / ip - konfiguracja i zarządzanie ustawieniami interface'ów sieciowych

ip addr

useradd
chmod
chown
env
echo $PATH
tail
hed

cronjob
jobs
bg %1
fg %1
screen - multiterminalowosc
screen -S nazwa
przechodzenie miedzy sesją - CTRL-A d

sprawdzic czy dziala na linuksie:
tracert onet.pl
nslookup google.pl
tcpdump -i eth0
nmap -v A adresip
