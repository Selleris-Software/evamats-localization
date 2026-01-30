# Workflow report
https://selleris-my.sharepoint.com/:x:/p/sd/IQCXFg2XxdncQbKyAgPIH6nPAXXrxi18lv4iHdDu7A087NM?e=cqIG9c


# 418	Wysyłanie e-maili- automatyzacja
## BLIK
### Wyślij wiadomość e-mail do klienta
``` html
<p>
Dzień dobry,<br>
dywaniki samochodowe EVAMATS, potwierdzenie zamówienia nr: {=Document:UF_CRM_1706355079}. Proszę o potwierdzenie modelu.
</p>
<p>
Marka Auta: {=Document:UF_CRM_633A9AFAA6955}, Model Auta: {=Document:UF_CRM_62BEB9DEEB6A7}, Silnik: {=Document:UF_CRM_1700125057018}, Napęd maszyny: {=Document:UF_CRM_1700124949859}, Skrzynia biegów: {=Document:UF_CRM_634430D33F3A4}, Rok produkcji: {=Document:UF_CRM_633A9AFB10E01}, Typ nadwozia: {=Document:UF_CRM_634430D32EE3C}, Ilość miejsc: {=Document:UF_CRM_634430D31273D}, Kraj pochodzenia: {=Document:UF_CRM_1700125125567}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631}<br>
Kształt: {=Document:UF_CRM_634430D349FE5}.<br>
Materiał: {=Document:UF_CRM_633A9AFB81D7C}.<br>
Obszycie: {=Document:UF_CRM_633A9AFBA136F}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631} - {=Variable:cenaKompletu > printable} zł. <br>
{=Variable:dodatki > printable}<br>
Koszt wysyłki - {=Document:UF_CRM_1677247963} zł.<br>
Razem do zapłaty: {=Document:OPPORTUNITY_ACCOUNT} zł.
</p>
<p>
Czas realizacji wynosi {=Variable:dostepnosc > printable}.<br>
Adres do wysyłki: {=Variable:adresDostawy > printable}.
</p>
<p>
Przekierowanie do płatności w wysokości {=Document:UF_CRM_1706299688 > double} zł, dostępne opcje płatności kartą, przelewy24 i BLIK, link jest ważny przez 24 godziny: {=Document:UF_CRM_1732194395}.<br>
Do zapłaty za pobraniem u kuriera pozostanie: {=Document:UF_CRM_1706121001 > double} zł.
</p>
<p>
Wszystkie informacje dotyczące {=Variable:pozdrowienie > printable} zamówienia zostały zawarte w danej wiadomości, w wypadku jeśli zauważyliście Państwo, brak należytej informacji w danym potwierdzeniu, prosimy o kontakt w celu potwierdzenia ustalonych szczegółów dotyczących zamówienia wiadomością potwierdzającą.<br>
<a href="https://evamats.pl/policies/terms-of-service">https://evamats.pl/policies/terms-of-service</a>
</p>
<p>
Dziękujemy za złożone zamówienie!</a><br>
W razie jakichkolwiek pytań pozostaję do dyspozycji! tel. {=Document:ASSIGNED_BY_WORK_PHONE}<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
<a href="https://evamats.pl/">www.evamats.pl</a>
</p>
<p>
Pozdrawiam serdecznie,<br>
zespół EVAMATS!
</p>
```
Pliki:
- https://evamats.bitrix24.pl/disk/file/bZpXp15muyG7fQpnaToo
- https://evamats.bitrix24.pl/disk/file/d7XQ3C6kE80baboGYoSW
- https://evamats.bitrix24.pl/disk/file/Mk7Fe7LhtheHJ4vxZhHl

### Wyślij SMS
``` html
EVAMATS – zamówienie nr: {{Nr zamówienia}}

{{Marka Auta}}, {{Model Auta}}, {{Rok produkcji}}, {{Typ nadwozia}}, {{Wariant kompletu}}, materiał: {{Kolor materiału}}, obszycie: {{Kolor obszycia}}.

{=Variable:rodzajKompletu > printable} {{Wariant kompletu}} - {=Variable:cenaKompletu > printable} zł.
{=Variable:dodatkiComment > printable}
Razem do zapłaty z dostawą: {{Kwota (w walucie księgowania)}} zł.
Dostawa: {=Variable:adresDostawy > printable}. 

Płatność online (ważna 24h): {{Link do płatności}}

Pełne potwierdzenie wysłane na e-mail.
Kontakt: {{Osoba odpowiedzialna (telefon służbowy)}}
```

## PRZELEW
### Wyślij wiadomość e-mail do klienta
``` html
EVAMATS – zamówienie  nr: {{Nr zamówienia}}

{{Marka Auta}}, {{Model Auta}}, {{Rok produkcji}}, {{Typ nadwozia}}, {{Wariant kompletu}}, materiał: {{Kolor materiału}}, obszycie: {{Kolor obszycia}}.

{=Variable:rodzajKompletu > printable} {{Wariant kompletu}} - {=Variable:cenaKompletu > printable} zł.
{=Variable:dodatkiComment > printable}
Razem do zapłaty z dostawą: {{Kwota (w walucie księgowania)}} zł.
Dostawa: {=Variable:adresDostawy > printable}.

Dane do płatności w wysokości {{Przedpłata dla EURO > double}} euro, w tytule prosimy o podanie numeru zamówienia: {{Nr zamówienia}}.
EVAMATS Sp. z o.o.  
Alior Bank
SWIFT: ALBPPLPW
IBAN: PL17 249000050000460067445675
17 2490 0005 0000 4600 6744 5675

Prosimy o potwierdzenie płatności w momencie dokonania przelewu.

Pełne potwierdzenie wysłane na e-mail.
Kontakt: {{Osoba odpowiedzialna (telefon służbowy)}}
<p>
Dzień dobry,<br>
dywaniki samochodowe EVAMATS, potwierdzenie zamówienia nr: {=Document:UF_CRM_1706355079}. Proszę o potwierdzenie modelu.
</p>
<p>
Marka Auta: {=Document:UF_CRM_633A9AFAA6955}, Model Auta: {=Document:UF_CRM_62BEB9DEEB6A7}, Silnik: {=Document:UF_CRM_1700125057018}, Napęd maszyny: {=Document:UF_CRM_1700124949859}, Skrzynia biegów: {=Document:UF_CRM_634430D33F3A4}, Rok produkcji: {=Document:UF_CRM_633A9AFB10E01}, Typ nadwozia: {=Document:UF_CRM_634430D32EE3C}, Ilość miejsc: {=Document:UF_CRM_634430D31273D}, Kraj pochodzenia: {=Document:UF_CRM_1700125125567}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631}.<br>
Kształt: {=Document:UF_CRM_634430D349FE5}.<br>
Materiał: {=Document:UF_CRM_633A9AFB81D7C}.<br>
Obszycie: {=Document:UF_CRM_633A9AFBA136F}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631} - {=Variable:cenaKompletu > printable} zł.<br>
{=Variable:dodatki > printable}<br>
Koszt wysyłki - {=Document:UF_CRM_1677247963} zł.<br>
Razem do zapłaty: {=Document:OPPORTUNITY_ACCOUNT} zł.
</p>
<p>
Czas realizacji wynosi {=Variable:dostepnosc > printable}. <br>
Adres do wysyłki: {=Variable:adresDostawy > printable}.
</p>
<p>
Dane do płatności w wysokości {=Document:UF_CRM_1706299688 > double} zł, w tytule prosimy o podanie numeru zamówienia: {=Document:UF_CRM_1706355079}.<br>
Alior bank<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
Numer konta: 78 2490 0005 0000 4530 1376 8507
</p>
<p>
Prosimy o potwierdzenie płatności w momencie dokonania przelewu.<br>
Do zapłaty za pobraniem u kuriera pozostanie: {=Document:UF_CRM_1706121001 > double} zł.
</p>
<p>
Wszystkie informacje dotyczące {=Variable:pozdrowienie > printable} zamówienia zostały zawarte w danej wiadomości, w wypadku jeśli zauważyliście Państwo, brak należytej informacji w danym potwierdzeniu, prosimy o kontakt w celu potwierdzenia ustalonych szczegółów dotyczących zamówienia wiadomością potwierdzającą.<br>
<a href="https://evamats.pl/policies/terms-of-service">https://evamats.pl/policies/terms-of-service</a>
</p>
<p>
Dziękujemy za złożone zamówienie!<br>
W razie jakichkolwiek pytań pozostaję do dyspozycji! tel. {=Document:ASSIGNED_BY_WORK_PHONE}<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
<a href="https://evamats.pl/">www.evamats.pl</a>
</p>
<p>
Pozdrawiam serdecznie,<br>
zespół EVAMATS!
</p>
```
Pliki:
- https://evamats.bitrix24.pl/disk/file/bZpXp15muyG7fQpnaToo
- https://evamats.bitrix24.pl/disk/file/d7XQ3C6kE80baboGYoSW
- https://evamats.bitrix24.pl/disk/file/Mk7Fe7LhtheHJ4vxZhHl

### Wyślij SMS
```html
EVAMATS – zamówienie  nr: {{Nr zamówienia}}

{{Marka Auta}}, {{Model Auta}}, {{Rok produkcji}}, {{Typ nadwozia}}, {{Wariant kompletu}}, materiał: {{Kolor materiału}}, obszycie: {{Kolor obszycia}}.

{=Variable:rodzajKompletu > printable} {{Wariant kompletu}} - {=Variable:cenaKompletu > printable} zł.
{=Variable:dodatkiComment > printable}
Razem do zapłaty z dostawą: {{Kwota (w walucie księgowania)}} zł.
Dostawa: {=Variable:adresDostawy > printable}.

Dane do płatności w wysokości {{Przedpłata > double}} zł, w tytule prosimy o podanie numeru zamówienia: {{Nr zamówienia}}.
Alior bank
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667
Numer konta: 78 2490 0005 0000 4530 1376 8507

Prosimy o potwierdzenie płatności w momencie dokonania przelewu.

Pełne potwierdzenie wysłane na e-mail.
Kontakt: {{Osoba odpowiedzialna (telefon służbowy)}}
```

## PRZELEW EURO
### Wyślij wiadomość e-mail do klienta
``` html
<p>
Dzień dobry, <br>
dywaniki samochodowe EVAMATS, potwierdzenie zamówienia nr: {=Document:UF_CRM_1706355079}. Proszę o potwierdzenie modelu.
</p>
<p>
Marka Auta: {=Document:UF_CRM_633A9AFAA6955}, Model Auta: {=Document:UF_CRM_62BEB9DEEB6A7}, Silnik: {=Document:UF_CRM_1700125057018},  Napęd maszyny: {=Document:UF_CRM_1700124949859}, Skrzynia biegów: {=Document:UF_CRM_634430D33F3A4}, Rok produkcji: {=Document:UF_CRM_633A9AFB10E01}, Typ nadwozia: {=Document:UF_CRM_634430D32EE3C}, Ilość miejsc: {=Document:UF_CRM_634430D31273D}, Kraj pochodzenia: {=Document:UF_CRM_1700125125567}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631}.<br>
Kształt: {=Document:UF_CRM_634430D349FE5}.<br>
Materiał: {=Document:UF_CRM_633A9AFB81D7C}.<br>
Obszycie: {=Document:UF_CRM_633A9AFBA136F}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631} - {=Variable:cenaKompletu > printable} zł.<br>
{=Variable:dodatki > printable}<br>
Koszt wysyłki - {=Document:UF_CRM_1677247963} zł.<br>
Razem do zapłaty: {=Document:OPPORTUNITY_ACCOUNT} zł.
</p>
<p>
Czas realizacji wynosi {=Variable:dostepnosc > printable}.<br>
Adres do wysyłki: {=Variable:adresDostawy > printable}.
</p>
<p>
Dane do płatności w wysokości {=Document:UF_CRM_1732217821 > double} euro, w tytule prosimy o podanie numeru zamówienia: {=Document:UF_CRM_1706355079}.<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk.<br>
Alior Bank<br>
SWIFT: ALBPPLPW<br> 
IBAN: PL17 249000050000460067445675<br> 
17 2490 0005 0000 4600 6744 5675
</p>
<p>
Prosimy o potwierdzenie płatności w momencie dokonania przelewu.
</p>
<p>
Wszystkie informacje dotyczące {=Variable:pozdrowienie > printable} zamówienia zostały zawarte w danej wiadomości, w wypadku jeśli zauważyliście Państwo, brak należytej informacji w danym potwierdzeniu, prosimy o kontakt w celu potwierdzenia ustalonych szczegółów dotyczących zamówienia wiadomością potwierdzającą.<br> 
<a href="https://evamats.pl/policies/terms-of-service">https://evamats.pl/policies/terms-of-service</a>
</p>
<p>
Dziękujemy za złożone zamówienie!<br> 
W razie jakichkolwiek pytań pozostaję do dyspozycji! tel. {=Document:ASSIGNED_BY_WORK_PHONE}<br> 
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
<a href="https://evamats.pl/">www.evamats.pl</a>
</p>
<p>
Pozdrawiam serdecznie,<br>
zespół EVAMATS!
</p>
```
Pliki: 
- https://evamats.bitrix24.pl/disk/file/bZpXp15muyG7fQpnaToo
- https://evamats.bitrix24.pl/disk/file/d7XQ3C6kE80baboGYoSW
- https://evamats.bitrix24.pl/disk/file/Mk7Fe7LhtheHJ4vxZhHl

### Wyślij SMS
```html
EVAMATS – zamówienie  nr: {{Nr zamówienia}}

{{Marka Auta}}, {{Model Auta}}, {{Rok produkcji}}, {{Typ nadwozia}}, {{Wariant kompletu}}, materiał: {{Kolor materiału}}, obszycie: {{Kolor obszycia}}.

{=Variable:rodzajKompletu > printable} {{Wariant kompletu}} - {=Variable:cenaKompletu > printable} zł.
{=Variable:dodatkiComment > printable}
Razem do zapłaty z dostawą: {{Kwota (w walucie księgowania)}} zł.
Dostawa: {=Variable:adresDostawy > printable}.

Dane do płatności w wysokości {{Przedpłata dla EURO > double}} euro, w tytule prosimy o podanie numeru zamówienia: {{Nr zamówienia}}.
EVAMATS Sp. z o.o.  
Alior Bank
SWIFT: ALBPPLPW
IBAN: PL17 249000050000460067445675
17 2490 0005 0000 4600 6744 5675

Prosimy o potwierdzenie płatności w momencie dokonania przelewu.

Pełne potwierdzenie wysłane na e-mail.
Kontakt: {{Osoba odpowiedzialna (telefon służbowy)}}
```

## BLIK/PRZELEW
### Wyślij wiadomość e-mail do klienta
``` html
<p>
Dzień dobry,<br>
dywaniki samochodowe EVAMATS, potwierdzenie zamówienia nr: {=Document:UF_CRM_1706355079}. Proszę o potwierdzenie modelu.
</p>
<p>
Marka Auta: {=Document:UF_CRM_633A9AFAA6955}, Model Auta: {=Document:UF_CRM_62BEB9DEEB6A7}, Silnik: {=Document:UF_CRM_1700125057018}, Napęd maszyny: {=Document:UF_CRM_1700124949859},  Skrzynia biegów: {=Document:UF_CRM_634430D33F3A4}, Rok produkcji: {=Document:UF_CRM_633A9AFB10E01}, Typ nadwozia: {=Document:UF_CRM_634430D32EE3C}, Ilość miejsc: {=Document:UF_CRM_634430D31273D}, Kraj pochodzenia: {=Document:UF_CRM_1700125125567}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631}.<br>
Kształt: {=Document:UF_CRM_634430D349FE5}.<br>
Materiał: {=Document:UF_CRM_633A9AFB81D7C}.<br>
Obszycie: {=Document:UF_CRM_633A9AFBA136F}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631} - {=Variable:cenaKompletu > printable} zł.<br>
{=Variable:dodatki > printable}<br>
Koszt wysyłki - {=Document:UF_CRM_1677247963} zł.<br>
Razem do zapłaty: {=Document:OPPORTUNITY_ACCOUNT} zł.
</p>
<p>
Czas realizacji wynosi {=Variable:dostepnosc > printable}.<br>
Adres do wysyłki: {=Variable:adresDostawy > printable}.
</p>
<p>
Przekierowanie do płatności w wysokości {=Document:UF_CRM_1706299688 > double} zł, dostępne opcje płatności kartą, przelewy24 i BLIK, link jest ważny przez 24 godziny: {=Document:UF_CRM_1732194395}.
</p>
<p>
lub
</p>
<p>
Dane do płatności w wysokości {=Document:UF_CRM_1706299688 > double} zł, w tytule prosimy o podanie numeru zamówienia: {=Document:UF_CRM_1706355079}<br>
Alior bank<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667
</p>
<p>
Numer konta: 78 2490 0005 0000 4530 1376 8507
</p>
<p>
Prosimy o potwierdzenie płatności w momencie dokonania przelewu.<br>
Do zapłaty za pobraniem u kuriera pozostanie: {=Document:UF_CRM_1706121001  > double} zł.
</p>
<p>
Wszystkie informacje dotyczące {=Variable:pozdrowienie > printable} zamówienia zostały zawarte w danej wiadomości, w wypadku jeśli zauważyliście Państwo, brak należytej informacji w danym potwierdzeniu, prosimy o kontakt w celu potwierdzenia ustalonych szczegółów dotyczących zamówienia wiadomością potwierdzającą.<br>
<a href="https://evamats.pl/policies/terms-of-service">https://evamats.pl/policies/terms-of-service</a>
</p>
<p>
Dziękujemy za złożone zamówienie!<br>
W razie jakichkolwiek pytań pozostaję do dyspozycji! tel. {=Document:ASSIGNED_BY_WORK_PHONE}<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
<a href="https://evamats.pl/">www.evamats.pl</a>
</p>
<p>
Pozdrawiam serdecznie,<br>
zespół EVAMATS!
</p>
```
Pliki:
- https://evamats.bitrix24.pl/disk/file/bZpXp15muyG7fQpnaToo
- https://evamats.bitrix24.pl/disk/file/d7XQ3C6kE80baboGYoSW
- https://evamats.bitrix24.pl/disk/file/Mk7Fe7LhtheHJ4vxZhHl

### Wyślij SMS
``` html
EVAMATS – zamówienie nr: {{Nr zamówienia}}

{{Marka Auta}}, {{Model Auta}}, {{Rok produkcji}}, {{Typ nadwozia}}, {{Wariant kompletu}}, materiał: {{Kolor materiału}}, obszycie: {{Kolor obszycia}}.

{=Variable:rodzajKompletu > printable} {{Wariant kompletu}} - {=Variable:cenaKompletu > printable} zł.
{=Variable:dodatkiComment > printable}
Razem do zapłaty z dostawą: {{Kwota (w walucie księgowania)}} zł.
Dostawa: {=Variable:adresDostawy > printable}.

Płatność online (ważna 24h): {{Link do płatności}}

lub

Dane do płatności w wysokości {{Przedpłata > double}} zł, w tytule prosimy o podanie numeru zamówienia: {{Nr zamówienia}}.
Alior bank
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667
Numer konta: 78 2490 0005 0000 4530 1376 8507

Prosimy o potwierdzenie płatności w momencie dokonania przelewu.

Pełne potwierdzenie wysłane na e-mail.
Kontakt: {{Osoba odpowiedzialna (telefon służbowy)}}
```

## BLIK - Produkty
### Wyślij wiadomość e-mail do klienta
``` html
<p>
Dzień dobry,<br>
dywaniki samochodowe EVAMATS, potwierdzenie zamówienia nr: {=Document:UF_CRM_1706355079}. Proszę o potwierdzenie zamówienia.
</p>
<p>
{=Variable:dodatki > printable}<br>
Koszt wysyłki - {=Document:UF_CRM_1677247963} zł.<br>
Razem do zapłaty: {=Document:OPPORTUNITY_ACCOUNT} zł.
</p>
<p>
Czas realizacji wynosi około 3 dni.<br>
Adres do wysyłki: {=Variable:adresDostawy > printable}.
</p>
<p>
Przekierowanie do płatności w wysokości {=Document:UF_CRM_1706299688 > double} zł, dostępne opcje płatności kartą, przelewy24 i BLIK, link jest ważny przez 24 godziny: {=Document:UF_CRM_1732194395}.<br>
Do zapłaty za pobraniem u kuriera pozostanie: {=Document:UF_CRM_1706121001 > double} zł.
</p>
<p>
Wszystkie informacje dotyczące {=Variable:pozdrowienie > printable} zamówienia zostały zawarte w danej wiadomości, w wypadku jeśli zauważyliście Państwo, brak należytej informacji w danym potwierdzeniu, prosimy o kontakt w celu potwierdzenia ustalonych szczegółów dotyczących zamówienia wiadomością potwierdzającą.<br>
<a href="https://evamats.pl/policies/terms-of-service">https://evamats.pl/policies/terms-of-service</a>
</p>
<p>
Dziękujemy za złożone zamówienie!<br>
W razie jakichkolwiek pytań pozostaję do dyspozycji! tel. {=Document:ASSIGNED_BY_WORK_PHONE}<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
<a href="https://evamats.pl/">www.evamats.pl</a>
</p>
<p>
Pozdrawiam serdecznie,<br>
zespół EVAMATS!
</p>
```
Pliki:
- https://evamats.bitrix24.pl/disk/file/bZpXp15muyG7fQpnaToo
- https://evamats.bitrix24.pl/disk/file/d7XQ3C6kE80baboGYoSW
- https://evamats.bitrix24.pl/disk/file/Mk7Fe7LhtheHJ4vxZhHl

### Wyślij SMS
``` html
EVAMATS – zamówienie nr: {{Nr zamówienia}}

{=Variable:dodatkiComment > printable}:   zł.
Razem do zapłaty z dostawą: {{Kwota (w walucie księgowania)}} zł.

Czas realizacji wynosi około 3 dni.
Adres do wysyłki: {=Variable:adresDostawy > printable}.

Płatność online (ważna 24h): {{Link do płatności}}

Pełne potwierdzenie wysłane na e-mail.
Kontakt: {{Osoba odpowiedzialna (telefon służbowy)}}
```

## Opłata przy odbiorze - Produkty
### Wyślij wiadomość e-mail do klienta
``` html
<p>
Dzień dobry,<br>
dywaniki samochodowe EVAMATS, potwierdzenie zamówienia nr: {=Document:UF_CRM_1706355079}. Proszę o potwierdzenie zamówienia.
</p>
<p>
{=Variable:dodatki > printable}<br>
Koszt wysyłki - {=Document:UF_CRM_1677247963} zł.<br>
Razem do zapłaty: {=Document:OPPORTUNITY_ACCOUNT} zł.
</p>
<p>
Czas realizacji wynosi około 3 dni.<br>
Adres do wysyłki: {=Variable:adresDostawy > printable}.
</p>
<p>
Płatność: pobranie.<br>
Do zapłaty za pobraniem u kuriera pozostanie: {=Document:UF_CRM_1706121001 > double} zł.
</p>
<p>
Wszystkie informacje dotyczące {=Variable:pozdrowienie > printable} zamówienia zostały zawarte w danej wiadomości, w wypadku jeśli zauważyliście Państwo, brak należytej informacji w danym potwierdzeniu, prosimy o kontakt w celu potwierdzenia ustalonych szczegółów dotyczących zamówienia wiadomością potwierdzającą.<br>
<a href="https://evamats.pl/policies/terms-of-service">https://evamats.pl/policies/terms-of-service</a>
</p>
<p>
Dziękujemy za złożone zamówienie!</a><br>
W razie jakichkolwiek pytań pozostaję do dyspozycji! tel. {=Document:ASSIGNED_BY_WORK_PHONE}<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
<a href="https://evamats.pl/">www.evamats.pl</a>
</p>
<p>
Pozdrawiam serdecznie,<br>
zespół EVAMATS!
</p>
```
Pilki:
- https://evamats.bitrix24.pl/disk/file/bZpXp15muyG7fQpnaToo
- https://evamats.bitrix24.pl/disk/file/d7XQ3C6kE80baboGYoSW
- https://evamats.bitrix24.pl/disk/file/Mk7Fe7LhtheHJ4vxZhHl

### Wyślij SMS
``` html
EVAMATS – zamówienie nr: {{Nr zamówienia}}

{=Variable:dodatkiComment > printable}:   zł.
Razem do zapłaty z dostawą: {{Kwota (w walucie księgowania)}} zł.

Czas realizacji wynosi około 3 dni.
Adres do wysyłki: {=Variable:adresDostawy > printable}.

Płatność: pobranie.
Do zapłaty za pobraniem u kuriera pozostanie: {{Wartość pobrania > double}} zł.

Pełne potwierdzenie wysłane na e-mail.
Kontakt: {{Osoba odpowiedzialna (telefon służbowy)}}
```

## ZAKSIĘGOWANIE PŁATNOŚCI
### Wyślij wiadomość e-mail do klienta
``` html
<p>
Dzień dobry,<br>
dywaniki samochodowe EVAMATS, potwierdzenie zamówienia nr: {=Document:UF_CRM_1706355079}. Proszę o potwierdzenie modelu.
</p>
<p>
Marka Auta: {=Document:UF_CRM_633A9AFAA6955}, Model Auta: {=Document:UF_CRM_62BEB9DEEB6A7}, Silnik: {=Document:UF_CRM_1700125057018}, Napęd maszyny: {=Document:UF_CRM_1700124949859}, Skrzynia biegów: {=Document:UF_CRM_634430D33F3A4}, Rok produkcji: {=Document:UF_CRM_633A9AFB10E01}, Typ nadwozia: {=Document:UF_CRM_634430D32EE3C}, Ilość miejsc: {=Document:UF_CRM_634430D31273D}, Kraj pochodzenia: {=Document:UF_CRM_1700125125567}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631}.<br>
Kształt: {=Document:UF_CRM_634430D349FE5}.<br>
Materiał: {=Document:UF_CRM_633A9AFB81D7C}.<br>
Obszycie: {=Document:UF_CRM_633A9AFBA136F}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631} - {=Variable:cenaKompletu > printable} zł.<br>
{=Variable:dodatki > printable}<br>
Koszt wysyłki - {=Document:UF_CRM_1677247963} zł.<br>
Razem do zapłaty: {=Document:OPPORTUNITY_ACCOUNT} zł.
</p>
<p>
Czas realizacji wynosi {=Variable:dostepnosc > printable}. <br>
Adres do wysyłki: {=Variable:adresDostawy > printable}.
</p>
<p>
Potwierdzamy zaksięgowanie płatności w wysokości: {=Document:UF_CRM_1706299688 > double} zł,<br>
Do zapłaty przy odbiorze pozostanie: {=Document:UF_CRM_1706121001 > double} zł.
</p>
<p>
Wszystkie informacje dotyczące {=Variable:pozdrowienie > printable} zamówienia zostały zawarte w danej wiadomości, w wypadku jeśli zauważyliście Państwo, brak należytej informacji w danym potwierdzeniu, prosimy o kontakt w celu potwierdzenia ustalonych szczegółów dotyczących zamówienia wiadomością potwierdzającą.<br>
<a href="https://evamats.pl/policies/terms-of-service">https://evamats.pl/policies/terms-of-service</a>
</p>
<p>
Dziękujemy za złożone zamówienie!<br>
W razie jakichkolwiek pytań pozostaję do dyspozycji! tel. {=Document:ASSIGNED_BY_WORK_PHONE}<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
<a href="https://evamats.pl/">www.evamats.pl</a>
</p>
<p>
Pozdrawiam serdecznie,<br>
zespół EVAMATS!
</p>
```
Pilki:
- https://evamats.bitrix24.pl/disk/file/bZpXp15muyG7fQpnaToo
- https://evamats.bitrix24.pl/disk/file/d7XQ3C6kE80baboGYoSW
- https://evamats.bitrix24.pl/disk/file/Mk7Fe7LhtheHJ4vxZhHl

### Wyślij SMS
``` html
EVAMATS – zamówienie nr: {{Nr zamówienia}}

{{Marka Auta}}, {{Model Auta}}, {{Rok produkcji}}, {{Typ nadwozia}}, {{Wariant kompletu}}, materiał: {{Kolor materiału}}, obszycie: {{Kolor obszycia}}.

{=Variable:rodzajKompletu > printable} {{Wariant kompletu}} - {=Variable:cenaKompletu > printable} zł.
{=Variable:dodatkiComment > printable}
Razem do zapłaty z dostawą: {{Kwota (w walucie księgowania)}} zł.
Dostawa: {=Variable:adresDostawy > printable}.

Potwierdzamy zaksięgowanie płatności w wysokości: {{Przedpłata > double}} zł,
Do zapłaty przy odbiorze pozostanie:  {{Wartość pobrania > double}} zł.

Pełne potwierdzenie wysłane na e-mail.
Kontakt: {{Osoba odpowiedzialna (telefon służbowy)}}
```

## Domyślny
### Wyślij wiadomość e-mail do klienta
``` html
<p>
Dzień dobry,<br>
dywaniki samochodowe EVAMATS, potwierdzenie zamówienia nr: {=Document:UF_CRM_1706355079}. Proszę o potwierdzenie modelu.
</p>
<p>
Marka Auta: {=Document:UF_CRM_633A9AFAA6955}, Model Auta: {=Document:UF_CRM_62BEB9DEEB6A7}, Silnik: {=Document:UF_CRM_1700125057018}, Napęd maszyny: {=Document:UF_CRM_1700124949859},  Skrzynia biegów: {=Document:UF_CRM_634430D33F3A4}, Rok produkcji: {=Document:UF_CRM_633A9AFB10E01}, Typ nadwozia: {=Document:UF_CRM_634430D32EE3C}, Ilość miejsc: {=Document:UF_CRM_634430D31273D}, Kraj pochodzenia: {=Document:UF_CRM_1700125125567}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631}.<br>
Kształt: {=Document:UF_CRM_634430D349FE5}.<br>
Materiał: {=Document:UF_CRM_633A9AFB81D7C}.<br>
Obszycie: {=Document:UF_CRM_633A9AFBA136F}.
</p>
<p>
{=Variable:rodzajKompletu > printable} {=Document:UF_CRM_633A9AFA87631} - {=Variable:cenaKompletu > printable} zł.<br>
{{=explode(",", {=Variable:dodatki > printable})}}<br>
Koszt wysyłki - {=Document:UF_CRM_1677247963} zł.<br>
Razem do zapłaty: {=Document:OPPORTUNITY_ACCOUNT} zł.
</p>
<p>
Czas realizacji wynosi {=Variable:dostepnosc > printable}.<br>
Adres do wysyłki: {=Variable:adresDostawy > printable}.
</p>
<p>
Przekierowanie do płatności w wysokości {=Document:UF_CRM_1706299688 > double} zł, dostępne opcje płatności kartą, przelewy24 i BLIK, link jest ważny przez 24 godziny: {=Document:UF_CRM_1732194395}.
</p>
<p>
lub
</p>
<p>
Alior bank<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667
</p>
<p>
Numer konta: 78 2490 0005 0000 4530 1376 8507
</p>
<p>
Prosimy o potwierdzenie płatności gdy już dokona {=Document:CONTACT.HONORIFIC} przelewu.<br>
Do zapłaty za pobraniem u kuriera pozostanie: {=Document:UF_CRM_1706121001  > double} zł.
</p>
<p>
Wszystkie informacje dotyczące {=Variable:pozdrowienie > printable} zamówienia zostały zawarte w danej wiadomości, w wypadku jeśli zauważyliście Państwo, brak należytej informacji w danym potwierdzeniu, prosimy o kontakt w celu potwierdzenia ustalonych szczegółów dotyczących zamówienia wiadomością potwierdzającą.<br>
<a href="https://evamats.pl/policies/terms-of-service">https://evamats.pl/policies/terms-of-service</a>
</p>
<p>
Dziękujemy za złożone zamówienie!<br>
W razie jakichkolwiek pytań pozostaję do dyspozycji! tel. {=Document:ASSIGNED_BY_WORK_PHONE}<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
<a href="https://evamats.pl/">www.evamats.pl</a>
</p>
<p>
Pozdrawiam serdecznie,<br>
zespół EVAMATS!
</p>
```
Pilki:
- https://evamats.bitrix24.pl/disk/file/bZpXp15muyG7fQpnaToo
- https://evamats.bitrix24.pl/disk/file/d7XQ3C6kE80baboGYoSW
- https://evamats.bitrix24.pl/disk/file/Mk7Fe7LhtheHJ4vxZhHl

### Wyślij SMS
``` html
EVAMATS – zamówienie nr: {{Nr zamówienia}}

{{Marka Auta}}, {{Model Auta}}, {{Rok produkcji}}, {{Typ nadwozia}}, {{Wariant kompletu}}, materiał: {{Kolor materiału}}, obszycie: {{Kolor obszycia}}.

{=Variable:rodzajKompletu > printable} {{Wariant kompletu}} - {=Variable:cenaKompletu > printable} zł.
{=Variable:dodatkiComment > printable}
Razem do zapłaty z dostawą: {{Kwota (w walucie księgowania)}} zł.
Dostawa: {=Variable:adresDostawy > printable}.

Przekierowanie do płatności w wysokości {{Przedpłata > double}} zł, dostępne opcje płatności kartą, przelewy24 i BLIK, link jest ważny przez 24 godziny: {{Link do płatności}}.

lub

Alior bank
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667
Numer konta: 78 2490 0005 0000 4530 1376 8507

Prosimy o potwierdzenie płatności w momencie dokonania przelewu.

Pełne potwierdzenie wysłane na e-mail.
Kontakt: {{Osoba odpowiedzialna (telefon służbowy)}}
```


# 442	Wysyłanie email po stworzeniu e-paragona
## Is Email?
### Wyślij wiadomość e-mail do klienta
``` html 
<br>
<div id="main_mail_form_crm_mail_template_edit_form_14_quote_18e9edfad98">
 <br>
	<div>
		<div>
			 Witam,&nbsp;<br>
 <br>
			 Wysyłamy 
Eparagon {=Document:UF_CRM_1712848351} zgodnie z zamówieniem.&nbsp; Dziękuje&nbsp;<img src="https://fonts.gstatic.com/s/e/notoemoji/15.0/1f91d/72.png" style="height: 1.2em; width: 1.2em;"><br>
 <br>
 <br>
 <br>
			 Pozdrawiam<br>
 <br>
 <br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4xFYNHzggNeiLOZBHTRV1X4NUw0oaOg3qc-r7tfg3wxnyI0w6bwwbU17oje4xyBXd-UGJrmsyc"><br>
			<table cellpadding="0" cellspacing="0">
			<tbody>
			<tr>
				<td>
 <b>Maks Havryshchuk </b>
				</td>
			</tr>
			<tr>
				<td>
					 CEO &amp; Founder<br>
					 EVAMATS<br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4zNVi3ceiYsEP5YUnRp3Yoz0FUcs1YSMGpiQIU5tJLdnslr7y7YGzwMNn8boqdV4PG109bcavg"><br>
				</td>
			</tr>
			<tr>
				<td>
					 mobile:&nbsp;<a href="tel:+48730428913" target="_blank">+48</a>730428913<br>
 <a href="http://evamats.pl/" target="_blank">evamats.pl</a><br>
				</td>
			</tr>
			<tr>
				<td>
 <a href="https://www.facebook.com/evamatspl" target="_blank"><img width="200" alt="Facebook icon" src="https://ci5.googleusercontent.com/proxy/NNFToRb9IxBx1dGp0nj3RsJ_KKA5SWURBRes7oEUPV6-uq2N_dngJrIhk_GZZrap5o6oG2fMYgnRpojE5i_vVIeSos_jBWTLBZmoo25f2CsQ6CeVuly4AjtOepdChmDVItNRdYSRQ0c=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/fb.png" height="200" style="height: 20px; width: 20px;"></a><a href="https://www.instagram.com/evamats.pl" target="_blank"><img width="20" alt="Instagram icon" src="https://ci6.googleusercontent.com/proxy/hgT72ksYOS21Ucg4kyAl3BZZczs6GN60dJU18-F1duip2cJFueHNxu1R8TL5PGNXJr9Po_-yip82sywjecDjb1S6pWMijCkGK7kfXzjTHO-j0mu8Rza8PyqfhqEdscK5nNwz6KL_i84=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/it.png" height="20" style="height: 20px; width: 20px;"></a>&nbsp;&nbsp;
				</td>
			</tr>
			</tbody>
			</table>
 <br>
 <span style="font-size: 8pt;">Informacje zawarte w niniejszym przekazie elektronicznym mają charakter poufny i są przeznaczone wyłącznie dla adresata. Jeżeli nie są Państwo adresatem tego przekazu, prosimy powiadomić nadawcę o fakcie jego otrzymania, jak również zniszczyć ten przekaz wraz ze wszystkimi załącznikami, które zawiera. Wykorzystywanie do jakichkolwiek celów, ujawnianie, kopiowanie, zarówno w całości, jak i w części, informacji tu zawartych jest zabronione i stanowi naruszenie prawa. Zastrzegamy sobie prawo wglądu do treści każdego przekazu elektronicznego, który wpływa do naszych systemów elektronicznych lub jest z nich wysyłany.</span><br>
		</div>
 <br>
	</div>
 <br>
</div>
 <br>
 ```
Pilki:
-
-
-

### Wyślij SMS
``` html
EVAMATS: Wystawiono Eparagon do zamównienia

Witam,
Wysyłamy 
Eparagon {{Eparagon zaliczka link}} zgodnie z zamówieniem.
Dziękuje	 
Pozdrawiam
```


## Is Email?
### Wyślij wiadomość e-mail do klienta
``` html
<br>
<div id="main_mail_form_crm_mail_template_edit_form_14_quote_18e9edfad98">
 <br>
	<div>
		<div>
			 Witam,&nbsp;<br>
 <br>
			 Wysyłamy 
Eparagon {=Document:UF_CRM_1710937223} zgodnie z zamówieniem.&nbsp; Dziękuje&nbsp;<img src="https://fonts.gstatic.com/s/e/notoemoji/15.0/1f91d/72.png" style="height: 1.2em; width: 1.2em;"><br>
 <br>
 <br>
 <br>
			 Pozdrawiam<br>
 <br>
 <br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4xFYNHzggNeiLOZBHTRV1X4NUw0oaOg3qc-r7tfg3wxnyI0w6bwwbU17oje4xyBXd-UGJrmsyc"><br>
			<table cellpadding="0" cellspacing="0">
			<tbody>
			<tr>
				<td>
 <b>Maks Havryshchuk </b>
				</td>
			</tr>
			<tr>
				<td>
					 CEO &amp; Founder<br>
					 EVAMATS<br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4zNVi3ceiYsEP5YUnRp3Yoz0FUcs1YSMGpiQIU5tJLdnslr7y7YGzwMNn8boqdV4PG109bcavg"><br>
				</td>
			</tr>
			<tr>
				<td>
					 mobile:&nbsp;<a href="tel:+48730428913" target="_blank">+48</a>730428913<br>
 <a href="http://evamats.pl/" target="_blank">evamats.pl</a><br>
				</td>
			</tr>
			<tr>
				<td>
 <a href="https://www.facebook.com/evamatspl" target="_blank"><img width="200" alt="Facebook icon" src="https://ci5.googleusercontent.com/proxy/NNFToRb9IxBx1dGp0nj3RsJ_KKA5SWURBRes7oEUPV6-uq2N_dngJrIhk_GZZrap5o6oG2fMYgnRpojE5i_vVIeSos_jBWTLBZmoo25f2CsQ6CeVuly4AjtOepdChmDVItNRdYSRQ0c=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/fb.png" height="200" style="height: 20px; width: 20px;"></a><a href="https://www.instagram.com/evamats.pl" target="_blank"><img width="20" alt="Instagram icon" src="https://ci6.googleusercontent.com/proxy/hgT72ksYOS21Ucg4kyAl3BZZczs6GN60dJU18-F1duip2cJFueHNxu1R8TL5PGNXJr9Po_-yip82sywjecDjb1S6pWMijCkGK7kfXzjTHO-j0mu8Rza8PyqfhqEdscK5nNwz6KL_i84=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/it.png" height="20" style="height: 20px; width: 20px;"></a>&nbsp;&nbsp;
				</td>
			</tr>
			</tbody>
			</table>
 <br>
 <span style="font-size: 8pt;">Informacje zawarte w niniejszym przekazie elektronicznym mają charakter poufny i są przeznaczone wyłącznie dla adresata. Jeżeli nie są Państwo adresatem tego przekazu, prosimy powiadomić nadawcę o fakcie jego otrzymania, jak również zniszczyć ten przekaz wraz ze wszystkimi załącznikami, które zawiera. Wykorzystywanie do jakichkolwiek celów, ujawnianie, kopiowanie, zarówno w całości, jak i w części, informacji tu zawartych jest zabronione i stanowi naruszenie prawa. Zastrzegamy sobie prawo wglądu do treści każdego przekazu elektronicznego, który wpływa do naszych systemów elektronicznych lub jest z nich wysyłany.</span><br>
		</div>
 <br>
	</div>
 <br>
</div>
 <br>
```
Pliki:
-
-
-

### Wyślij SMS
``` html
EVAMATS: Wystawiono Eparagon do zamównienia

Witam,
Wysyłamy 
Eparagon {{Eparagon link}} zgodnie z zamówieniem.
Dziękuje	 
Pozdrawiam
```

## Is Email?
### Wyślij wiadomość e-mail do klienta
``` html
<br>
<div id="main_mail_form_crm_mail_template_edit_form_14_quote_18e9edfad98">
 <br>
	<div>
		<div>
			 Witam,&nbsp;<br>
 <br>
			 Wysyłamy 
Eparagon {=Document:UF_CRM_1710937223} zgodnie z zamówieniem.&nbsp; Dziękuje&nbsp;<img src="https://fonts.gstatic.com/s/e/notoemoji/15.0/1f91d/72.png" style="height: 1.2em; width: 1.2em;"><br>
 <br>
 <br>
 <br>
			 Pozdrawiam<br>
 <br>
 <br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4xFYNHzggNeiLOZBHTRV1X4NUw0oaOg3qc-r7tfg3wxnyI0w6bwwbU17oje4xyBXd-UGJrmsyc"><br>
			<table cellpadding="0" cellspacing="0">
			<tbody>
			<tr>
				<td>
 <b>Maks Havryshchuk </b>
				</td>
			</tr>
			<tr>
				<td>
					 CEO &amp; Founder<br>
					 EVAMATS<br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4zNVi3ceiYsEP5YUnRp3Yoz0FUcs1YSMGpiQIU5tJLdnslr7y7YGzwMNn8boqdV4PG109bcavg"><br>
				</td>
			</tr>
			<tr>
				<td>
					 mobile:&nbsp;<a href="tel:+48730428913" target="_blank">+48</a>730428913<br>
 <a href="http://evamats.pl/" target="_blank">evamats.pl</a><br>
				</td>
			</tr>
			<tr>
				<td>
 <a href="https://www.facebook.com/evamatspl" target="_blank"><img width="200" alt="Facebook icon" src="https://ci5.googleusercontent.com/proxy/NNFToRb9IxBx1dGp0nj3RsJ_KKA5SWURBRes7oEUPV6-uq2N_dngJrIhk_GZZrap5o6oG2fMYgnRpojE5i_vVIeSos_jBWTLBZmoo25f2CsQ6CeVuly4AjtOepdChmDVItNRdYSRQ0c=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/fb.png" height="200" style="height: 20px; width: 20px;"></a><a href="https://www.instagram.com/evamats.pl" target="_blank"><img width="20" alt="Instagram icon" src="https://ci6.googleusercontent.com/proxy/hgT72ksYOS21Ucg4kyAl3BZZczs6GN60dJU18-F1duip2cJFueHNxu1R8TL5PGNXJr9Po_-yip82sywjecDjb1S6pWMijCkGK7kfXzjTHO-j0mu8Rza8PyqfhqEdscK5nNwz6KL_i84=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/it.png" height="20" style="height: 20px; width: 20px;"></a>&nbsp;&nbsp;
				</td>
			</tr>
			</tbody>
			</table>
 <br>
 <span style="font-size: 8pt;">Informacje zawarte w niniejszym przekazie elektronicznym mają charakter poufny i są przeznaczone wyłącznie dla adresata. Jeżeli nie są Państwo adresatem tego przekazu, prosimy powiadomić nadawcę o fakcie jego otrzymania, jak również zniszczyć ten przekaz wraz ze wszystkimi załącznikami, które zawiera. Wykorzystywanie do jakichkolwiek celów, ujawnianie, kopiowanie, zarówno w całości, jak i w części, informacji tu zawartych jest zabronione i stanowi naruszenie prawa. Zastrzegamy sobie prawo wglądu do treści każdego przekazu elektronicznego, który wpływa do naszych systemów elektronicznych lub jest z nich wysyłany.</span><br>
		</div>
 <br>
	</div>
 <br>
</div>
 <br>
```
Pilki:
-
-
-

### Wyślij SMS
``` html
EVAMATS: Wystawiono Eparagon do zamównienia

Witam,
Wysyłamy 
Eparagon {{Eparagon link}} zgodnie z zamówieniem.
Dziękuje	 
Pozdrawiam
```




# 446	Wysyłanie email po stworzeniu faktury
## Is Email?
### Wyślij SMS
``` html
EVAMATS - Dywaniki samochodowe
Faktura Zaliczkowa.
Witam, 
Wysyłamy Panu/i link do faktury zgodnie z zamówieniem:
{{Faktura zaliczkowa link}}

Dziękuję 
Pozdrawiam
```

## Is Email?
### Wyślij wiadomość e-mail do klienta
``` html
<div id="main_mail_form_crm_mail_template_edit_form_16_quote_18f5ccdb571">
	<br>
	<div>
		<div>
			<div>
			</div>
			 Witam,&nbsp;<br>
 <br>
			 Wysyłamy Panu/i fakturę zgodnie z Pana/i zamówieniem.&nbsp;&nbsp;Dziękuje&nbsp;<img src="https://fonts.gstatic.com/s/e/notoemoji/15.0/1f91d/72.png" style="height: 1.2em; width: 1.2em;"><br>
 <br>
 <br>
 <br>
			 Pozdrawiam<br>
 <br>
 <br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4xFYNHzggNeiLOZBHTRV1X4NUw0oaOg3qc-r7tfg3wxnyI0w6bwwbU17oje4xyBXd-UGJrmsyc"><br>
			<table cellpadding="0" cellspacing="0">
			<tbody>
			<tr>
				<td>
 <b>Maks Havryshchuk </b>
				</td>
			</tr>
			<tr>
				<td>
					 CEO &amp; Founder<br>
					 EVAMATS<br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4zNVi3ceiYsEP5YUnRp3Yoz0FUcs1YSMGpiQIU5tJLdnslr7y7YGzwMNn8boqdV4PG109bcavg"><br>
				</td>
			</tr>
			<tr>
				<td>
					 mobile:&nbsp;<a href="tel:+48732082512" target="_blank">+48</a>732082512<br>
 <a href="http://evamats.pl/" target="_blank">evamats.pl</a><br>
				</td>
			</tr>
			<tr>
				<td>
 <a href="https://www.facebook.com/evamatspl" target="_blank"><img width="200" alt="Facebook icon" src="https://ci5.googleusercontent.com/proxy/NNFToRb9IxBx1dGp0nj3RsJ_KKA5SWURBRes7oEUPV6-uq2N_dngJrIhk_GZZrap5o6oG2fMYgnRpojE5i_vVIeSos_jBWTLBZmoo25f2CsQ6CeVuly4AjtOepdChmDVItNRdYSRQ0c=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/fb.png" height="200" style="height: 20px; width: 20px;"></a><a href="https://www.instagram.com/evamats.pl" target="_blank"><img width="20" alt="Instagram icon" src="https://ci6.googleusercontent.com/proxy/hgT72ksYOS21Ucg4kyAl3BZZczs6GN60dJU18-F1duip2cJFueHNxu1R8TL5PGNXJr9Po_-yip82sywjecDjb1S6pWMijCkGK7kfXzjTHO-j0mu8Rza8PyqfhqEdscK5nNwz6KL_i84=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/it.png" height="20" style="height: 20px; width: 20px;"></a>&nbsp;&nbsp;
				</td>
			</tr>
			</tbody>
			</table>
 <br>
 <span style="font-size: 8pt;">Informacje zawarte w niniejszym przekazie elektronicznym mają charakter poufny i są przeznaczone wyłącznie dla adresata. Jeżeli nie są Państwo adresatem tego przekazu, prosimy powiadomić nadawcę o fakcie jego otrzymania, jak również zniszczyć ten przekaz wraz ze wszystkimi załącznikami, które zawiera. Wykorzystywanie do jakichkolwiek celów, ujawnianie, kopiowanie, zarówno w całości, jak i w części, informacji tu zawartych jest zabronione i stanowi naruszenie prawa. Zastrzegamy sobie prawo wglądu do treści każdego przekazu elektronicznego, który wpływa do naszych systemów elektronicznych lub jest z nich wysyłany.</span><br>
		</div>
 <br>
	</div>
 <br>
</div>
<br>
```
Pilki: 
{{Faktura proforma pdf}}

## Is Email?
### Wyślij SMS
``` html
EVAMATS - Dywaniki samochodowe
Faktura PROFORMA.

Witam, 
Wysyłamy Panu/i link do faktury zgodnie z zamówieniem:
{{Faktura proforma link}}

Dziękuję 
Pozdrawiam
```
## Is Email?
### Wyślij wiadomość e-mail do klienta
``` html
<div id="main_mail_form_crm_mail_template_edit_form_16_quote_18f5ccdb571">
	<br>
	<div>
		<div>
			<div>
			</div>
			 Witam,&nbsp;<br>
 <br>
			 Wysyłamy Panu/i fakturę zgodnie z Pana/i zamówieniem.&nbsp;&nbsp; Po otrzymaniu potwierdzenia przelewu, projekt zostanie przekazany do realizacji. Dziękuje &nbsp;<img src="https://fonts.gstatic.com/s/e/notoemoji/15.0/1f91d/72.png" style="height: 1.2em; width: 1.2em;"><br>
 <br>
 <br>
 <br>
			 Pozdrawiam<br>
 <br>
 <br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4xFYNHzggNeiLOZBHTRV1X4NUw0oaOg3qc-r7tfg3wxnyI0w6bwwbU17oje4xyBXd-UGJrmsyc"><br>
			<table cellpadding="0" cellspacing="0">
			<tbody>
			<tr>
				<td>
 <b>Maks Havryshchuk </b>
				</td>
			</tr>
			<tr>
				<td>
					 CEO &amp; Founder<br>
					 EVAMATS<br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4zNVi3ceiYsEP5YUnRp3Yoz0FUcs1YSMGpiQIU5tJLdnslr7y7YGzwMNn8boqdV4PG109bcavg"><br>
				</td>
			</tr>
			<tr>
				<td>
					 mobile:&nbsp;<a href="tel:+48732082512" target="_blank">+48</a>732082512<br>
 <a href="http://evamats.pl/" target="_blank">evamats.pl</a><br>
				</td>
			</tr>
			<tr>
				<td>
 <a href="https://www.facebook.com/evamatspl" target="_blank"><img width="200" alt="Facebook icon" src="https://ci5.googleusercontent.com/proxy/NNFToRb9IxBx1dGp0nj3RsJ_KKA5SWURBRes7oEUPV6-uq2N_dngJrIhk_GZZrap5o6oG2fMYgnRpojE5i_vVIeSos_jBWTLBZmoo25f2CsQ6CeVuly4AjtOepdChmDVItNRdYSRQ0c=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/fb.png" height="200" style="height: 20px; width: 20px;"></a><a href="https://www.instagram.com/evamats.pl" target="_blank"><img width="20" alt="Instagram icon" src="https://ci6.googleusercontent.com/proxy/hgT72ksYOS21Ucg4kyAl3BZZczs6GN60dJU18-F1duip2cJFueHNxu1R8TL5PGNXJr9Po_-yip82sywjecDjb1S6pWMijCkGK7kfXzjTHO-j0mu8Rza8PyqfhqEdscK5nNwz6KL_i84=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/it.png" height="20" style="height: 20px; width: 20px;"></a>&nbsp;&nbsp;
				</td>
			</tr>
			</tbody>
			</table>
 <br>
 <span style="font-size: 8pt;">Informacje zawarte w niniejszym przekazie elektronicznym mają charakter poufny i są przeznaczone wyłącznie dla adresata. Jeżeli nie są Państwo adresatem tego przekazu, prosimy powiadomić nadawcę o fakcie jego otrzymania, jak również zniszczyć ten przekaz wraz ze wszystkimi załącznikami, które zawiera. Wykorzystywanie do jakichkolwiek celów, ujawnianie, kopiowanie, zarówno w całości, jak i w części, informacji tu zawartych jest zabronione i stanowi naruszenie prawa. Zastrzegamy sobie prawo wglądu do treści każdego przekazu elektronicznego, który wpływa do naszych systemów elektronicznych lub jest z nich wysyłany.</span><br>
		</div>
 <br>
	</div>
 <br>
</div>
<br>
```
Pilki: 
{{Faktura proforma pdf}}

## Is Email?
### Wyślij SMS
``` html
EVAMATS - Dywaniki samochodowe
Faktura VAT;

Witam, 
Wysyłamy Panu/i link do faktury zgodnie z zamówieniem:
{{Faktura link(fakturownia.pl)}}

Dziękuję 
Pozdrawiam
```

## Is Email?
### Wyślij wiadomość e-mail do klienta
``` html
<div id="main_mail_form_crm_mail_template_edit_form_16_quote_18f5ccdb571">
	<br>
	<div>
		<div>
			<div>
			</div>
			 Witam,&nbsp;<br>
 <br>
			 Wysyłamy Panu/i fakturę zgodnie z Pana/i zamówieniem.&nbsp;&nbsp;Dziękuje&nbsp;<img src="https://fonts.gstatic.com/s/e/notoemoji/15.0/1f91d/72.png" style="height: 1.2em; width: 1.2em;"><br>
 <br>
 <br>
 <br>
			 Pozdrawiam<br>
 <br>
 <br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4xFYNHzggNeiLOZBHTRV1X4NUw0oaOg3qc-r7tfg3wxnyI0w6bwwbU17oje4xyBXd-UGJrmsyc"><br>
			<table cellpadding="0" cellspacing="0">
			<tbody>
			<tr>
				<td>
 <b>Maks Havryshchuk </b>
				</td>
			</tr>
			<tr>
				<td>
					 CEO &amp; Founder<br>
					 EVAMATS<br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4zNVi3ceiYsEP5YUnRp3Yoz0FUcs1YSMGpiQIU5tJLdnslr7y7YGzwMNn8boqdV4PG109bcavg"><br>
				</td>
			</tr>
			<tr>
				<td>
					 mobile:&nbsp;<a href="tel:+48732082512" target="_blank">+48</a>732082512<br>
 <a href="http://evamats.pl/" target="_blank">evamats.pl</a><br>
				</td>
			</tr>
			<tr>
				<td>
 <a href="https://www.facebook.com/evamatspl" target="_blank"><img width="200" alt="Facebook icon" src="https://ci5.googleusercontent.com/proxy/NNFToRb9IxBx1dGp0nj3RsJ_KKA5SWURBRes7oEUPV6-uq2N_dngJrIhk_GZZrap5o6oG2fMYgnRpojE5i_vVIeSos_jBWTLBZmoo25f2CsQ6CeVuly4AjtOepdChmDVItNRdYSRQ0c=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/fb.png" height="200" style="height: 20px; width: 20px;"></a><a href="https://www.instagram.com/evamats.pl" target="_blank"><img width="20" alt="Instagram icon" src="https://ci6.googleusercontent.com/proxy/hgT72ksYOS21Ucg4kyAl3BZZczs6GN60dJU18-F1duip2cJFueHNxu1R8TL5PGNXJr9Po_-yip82sywjecDjb1S6pWMijCkGK7kfXzjTHO-j0mu8Rza8PyqfhqEdscK5nNwz6KL_i84=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/it.png" height="20" style="height: 20px; width: 20px;"></a>&nbsp;&nbsp;
				</td>
			</tr>
			</tbody>
			</table>
 <br>
 <span style="font-size: 8pt;">Informacje zawarte w niniejszym przekazie elektronicznym mają charakter poufny i są przeznaczone wyłącznie dla adresata. Jeżeli nie są Państwo adresatem tego przekazu, prosimy powiadomić nadawcę o fakcie jego otrzymania, jak również zniszczyć ten przekaz wraz ze wszystkimi załącznikami, które zawiera. Wykorzystywanie do jakichkolwiek celów, ujawnianie, kopiowanie, zarówno w całości, jak i w części, informacji tu zawartych jest zabronione i stanowi naruszenie prawa. Zastrzegamy sobie prawo wglądu do treści każdego przekazu elektronicznego, który wpływa do naszych systemów elektronicznych lub jest z nich wysyłany.</span><br>
		</div>
 <br>
	</div>
 <br>
</div>
<br>
```
Pilki:
{{Faktura pdf}}

## Is Email?
### Wyślij SMS
``` html
EVAMATS - Dywaniki samochodowe
Faktura KOŃCOWA; 

Witam, 
Wysyłamy Panu/i link do faktury zgodnie z zamówieniem:
{{Faktura link(fakturownia.pl)}}

Dziękuję 
Pozdrawiam
```

## Is Email?
### Wyślij wiadomość e-mail do klienta
``` html
<div id="main_mail_form_crm_mail_template_edit_form_16_quote_18f5ccdb571">
	<br>
	<div>
		<div>
			<div>
			</div>
			 Witam,&nbsp;<br>
 <br>
			 Wysyłamy Panu/i fakturę zgodnie z Pana/i zamówieniem.&nbsp;&nbsp;Opłata pozostałej kwoty będzie przy odbiorze Pana zamówienia. Fakturę wysyłamy już teraz a opłata u kuriera. Dziękuje&nbsp;<img src="https://fonts.gstatic.com/s/e/notoemoji/15.0/1f91d/72.png" style="height: 1.2em; width: 1.2em;"><br>
 <br>
 <br>
 <br>
			 Pozdrawiam<br>
 <br>
 <br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4xFYNHzggNeiLOZBHTRV1X4NUw0oaOg3qc-r7tfg3wxnyI0w6bwwbU17oje4xyBXd-UGJrmsyc"><br>
			<table cellpadding="0" cellspacing="0">
			<tbody>
			<tr>
				<td>
 <b>Maks Havryshchuk </b>
				</td>
			</tr>
			<tr>
				<td>
					 CEO &amp; Founder<br>
					 EVAMATS<br>
 <img src="https://ci3.googleusercontent.com/mail-sig/AIorK4zNVi3ceiYsEP5YUnRp3Yoz0FUcs1YSMGpiQIU5tJLdnslr7y7YGzwMNn8boqdV4PG109bcavg"><br>
				</td>
			</tr>
			<tr>
				<td>
					 mobile:&nbsp;<a href="tel:+48732082512" target="_blank">+48</a>732082512<br>
 <a href="http://evamats.pl/" target="_blank">evamats.pl</a><br>
				</td>
			</tr>
			<tr>
				<td>
 <a href="https://www.facebook.com/evamatspl" target="_blank"><img width="200" alt="Facebook icon" src="https://ci5.googleusercontent.com/proxy/NNFToRb9IxBx1dGp0nj3RsJ_KKA5SWURBRes7oEUPV6-uq2N_dngJrIhk_GZZrap5o6oG2fMYgnRpojE5i_vVIeSos_jBWTLBZmoo25f2CsQ6CeVuly4AjtOepdChmDVItNRdYSRQ0c=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/fb.png" height="200" style="height: 20px; width: 20px;"></a><a href="https://www.instagram.com/evamats.pl" target="_blank"><img width="20" alt="Instagram icon" src="https://ci6.googleusercontent.com/proxy/hgT72ksYOS21Ucg4kyAl3BZZczs6GN60dJU18-F1duip2cJFueHNxu1R8TL5PGNXJr9Po_-yip82sywjecDjb1S6pWMijCkGK7kfXzjTHO-j0mu8Rza8PyqfhqEdscK5nNwz6KL_i84=s0-d-e1-ft#https://www.mail-signatures.com/signature-generator/img/templates/elegant-logo/it.png" height="20" style="height: 20px; width: 20px;"></a>&nbsp;&nbsp;
				</td>
			</tr>
			</tbody>
			</table>
 <br>
 <span style="font-size: 8pt;">Informacje zawarte w niniejszym przekazie elektronicznym mają charakter poufny i są przeznaczone wyłącznie dla adresata. Jeżeli nie są Państwo adresatem tego przekazu, prosimy powiadomić nadawcę o fakcie jego otrzymania, jak również zniszczyć ten przekaz wraz ze wszystkimi załącznikami, które zawiera. Wykorzystywanie do jakichkolwiek celów, ujawnianie, kopiowanie, zarówno w całości, jak i w części, informacji tu zawartych jest zabronione i stanowi naruszenie prawa. Zastrzegamy sobie prawo wglądu do treści każdego przekazu elektronicznego, który wpływa do naszych systemów elektronicznych lub jest z nich wysyłany.</span><br>
		</div>
 <br>
	</div>
 <br>
</div>
<br>
```
Pilki: 
{{Faktura pdf}}



# 498	Wysłanie komunikacji "Czekam na opłatę"
## Is Email?
### Wyślij wiadomość e-mail do klienta
``` html
<p>
Dzień dobry!😃
Dziękujemy za złożenie zamówienia na dywaniki samochodowe EVAMATS! Już niebawem dywaniki będą właśnie u ciebie i będziesz mógł się cieszyć ich użytkowaniem!<br>
</p>
<p>
Twoje zamówienie jest właśnie w trakcie realizacji na produkcji. Niezmiernie prosimy o dokonania ustalonej płatności abyśmy mogli dokończyć szycie i wysłać twoje dywaniki, ponieważ zależy nam na wywiązaniu się z warunków umowy, którą zawarliśmy podczas składania zamówienia.
</p>
<p>
Swoje zamówienie możesz opłacić poniżej:👇🏻<br>
Przekierowanie do płatności w wysokości {=Document:UF_CRM_1706299688 > double} zł, dostępne opcje płatności kartą, przelewy24 i BLIK, link jest ważny przez 24 godziny: {=Document:UF_CRM_1732194395}
</p>
<p>
Czekamy na szybkie zaksięgowanie płatności i wysyłamy twoje dywaniki EVAMATS!<br>
W razie jakichkolwiek pytań pozostaję do dyspozycji! tel {=Document:ASSIGNED_BY_WORK_PHONE}<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
<a href="https://evamats.pl/">www.evamats.pl</a>
</p>
<p>
Pozdrawiam serdecznie,<br>
zespół EVAMATS!
</p>
```

### Send SMS
``` html
Dzień dobry! Twoje zamówienie jest w trakcie realizacji, prosimy o szybką kontynuację płatności, aby dokończyć szycie:

Przekierowanie do płatności w wysokości {{Przedpłata > double}} zł, dostępne opcje płatności kartą, przelewy24 i BLIK, link jest ważny przez 24 godziny: {{Link do płatności}}

Czekamy na szybkie zaksięgowanie płatności i wysyłamy twoje dywaniki EVAMATS!

Pozdrawiam serdecznie, zespół EVAMATS!
```

## Is Email?
### Send email to customer
``` html
<p>
Dzień dobry!😃
Dziękujemy za złożenie zamówienia na dywaniki samochodowe EVAMATS! Już niebawem dywaniki będą właśnie u ciebie i będziesz mógł się cieszyć ich użytkowaniem!<br>
</p>
<p>
Twoje zamówienie jest właśnie w trakcie realizacji na produkcji. Niezmiernie prosimy o dokonania ustalonej płatności abyśmy mogli dokończyć szycie i wysłać twoje dywaniki, ponieważ zależy nam na wywiązaniu się z warunków umowy, którą zawarliśmy podczas składania zamówienia.
</p>
<p>
Swoje zamówienie możesz opłacić poniżej:👇🏻<br>
Dane do płatności w wysokości {=Document:UF_CRM_1706299688 > double} zł, w tytule prosimy o podanie numeru zamówienia: {=Document:UF_CRM_1706355079}.<br>
Alior bank<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
Numer konta: 78 2490 0005 0000 4530 1376 8507
</p>
<p>
Czekamy na szybkie zaksięgowanie płatności i wysyłamy twoje dywaniki EVAMATS!<br>
W razie jakichkolwiek pytań pozostaję do dyspozycji! tel {=Document:ASSIGNED_BY_WORK_PHONE}<br>
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667<br>
<a href="https://evamats.pl/">www.evamats.pl</a>
</p>
<p>
Pozdrawiam serdecznie,<br>
zespół EVAMATS!
</p>
```

### Send SMS
``` html 
Dzień dobry! Twoje zamówienie jest w trakcie realizacji, prosimy o szybką kontynuację płatności, aby dokończyć szycie:

Dane do płatności w wysokości {{Przedpłata > double}} zł, w tytule prosimy o podanie numeru zamówienia: {{Nr zamówienia}}.
Alior bank
EVAMATS Sp. z o.o.   ul. Strzelca 42,  80-299 Gdańsk, NIP: 5862378667
Numer konta: 78 2490 0005 0000 4530 1376 8507

Czekamy na szybkie zaksięgowanie płatności i wysyłamy twoje dywaniki EVAMATS!

Pozdrawiam serdecznie, zespół EVAMATS!
```




# 550	Wezwanie przedsądowe
## Is Email?
### Send email to customer
``` html
Szanowni Państwo,

w załączniku przesyłamy oficjalne wezwanie do zapłaty.

Brak uregulowania płatności w wyznaczonym terminie może skutkować przekazaniem sprawy do windykacji lub postępowania sądowego.

Prosimy o zapoznanie się z dokumentem i niezwłoczne uregulowanie należności.
```
Pilki: {=A74251_43328_97648_72365:DocumentPdf}





# 718	Workflou dla etapu "Informacja zwrotna"
## Is Email?
### Wyślij e-mail
``` html
<div style="font-family: Arial, sans-serif; font-size:14px; line-height:1.5; color:#333333;">

  <p>Witam serdecznie 👋</p>

  <p>Twoje dywaniki już wyruszyły w drogę 😀</p>

  <p>
    Jakość naszego produktu najlepiej mogą ocenić tylko nasi klienci, dlatego my cały czas
    monitorujemy i analizujemy opinie od Was. Dzięki temu możemy dopracować nasz produkt do ideału.
  </p>

  <p>
    Gdyby była taka możliwość, prosimy również o przesłanie drogą mailową zdjęć dywaników
    w Pana/Pani samochodzie 🙂
  </p>

  <p>
    Nasza strona internetowa:
    <a href="https://evamats.pl/" target="_blank">evamats.pl</a>
  </p>

  <p><strong>Instrukcje montażu akcesoriów EVAMATS</strong></p>

  <p>
    Montaż podpiętki metalowej
    <a href="https://www.youtube.com/watch?v=TTpWl_mdV28" target="_blank">Zobacz film instruktażowy</a><br>
    Montaż podpiętki EVAMATS
    <a href="https://www.youtube.com/watch?v=DUBcfAFtsSM" target="_blank">Zobacz film instruktażowy</a><br>
    Montaż podpiętki plastikowej EVAMATS
    <a href="https://www.youtube.com/watch?v=gyuYMWTWRwY" target="_blank">Zobacz film instruktażowy</a><br>
    Montaż podpiętki gumowej
    <a href="https://www.youtube.com/watch?v=lugnrSUagXI" target="_blank">Zobacz film instruktażowy</a><br>
    Jak prawidłowo przykleić rzep samoprzylepny
    <a href="https://www.youtube.com/watch?v=bi_7veXM_ZU" target="_blank">Zobacz film instruktażowy</a><br>
    Montaż tunelu środkowego
    <a href="https://www.youtube.com/watch?v=edxis2bdrrg" target="_blank">Zobacz film instruktażowy</a><br>
    Montaż dywanika z mocowaniem typu „haczyk”
    <a href="https://www.youtube.com/watch?v=hBxOy6Px5AI" target="_blank">Zobacz film instruktażowy</a>
  </p>

  <p>
    Mamy nadzieję, że nasze dywaniki spodobają się Panu/Pani i będą służyć dłużej, niż zakładamy!
  </p>

  <p>Pozdrawiam serdecznie,</p>

  <p>
    Zespół<br>
    <strong>EVAMATS</strong><br><br>
    <a href="tel:+48732082512">+48 732 082 512</a><br>
    <a href="https://evamats.pl/" target="_blank">evamats.pl</a><br><br>
    <a href="https://www.facebook.com/evamatspl" target="_blank">Facebook</a> |
    <a href="https://www.instagram.com/evamats.pl" target="_blank">Instagram</a>
  </p>

  <p style="font-size:12px; color:#777777; margin-top:20px;">
    Informacje zawarte w niniejszym przekazie elektronicznym mają charakter poufny i są przeznaczone wyłącznie dla adresata.
    Jeżeli nie są Państwo adresatem tego przekazu, prosimy powiadomić nadawcę o fakcie jego otrzymania, jak również zniszczyć
    ten przekaz wraz ze wszystkimi załącznikami, które zawiera. Wykorzystywanie do jakichkolwiek celów, ujawnianie, kopiowanie,
    zarówno w całości, jak i w części, informacji tu zawartych jest zabronione i stanowi naruszenie prawa. Zastrzegamy sobie
    prawo wglądu do treści każdego przekazu elektronicznego, który wpływa do naszych systemów elektronicznych lub jest z nich wysyłany.
  </p>

</div>
```

## Is Email?
### Wyślij SMS
``` html
Witam serdecznie👋
Dziękuję za korzystanie z dywaników EVAMATS 😊
Byłbym bardzo wdzięczny za opinię o naszych dywanikach na Google map  https://goo.gl/maps/EuxQDbghqWuiDQ239

Dziękuję!
Maks EVAMATS
```


# 766	Akceptacja kompletów: Potwierdzenie otrzymania zdjęć
## Is Email?
### Wyślij SMS
``` html
Potwierdzamy otrzymanie zdjęć podłogi. Materiały zostały przekazane do produkcji, zamówienie jest w trakcie realizacji. Dziękujemy!
```

### Wyślij e-mail
``` html
<p>
Dzień dobry,
</p>
<p>
dziękujemy za przesłanie zdjęć podłogi w pojeździe — <b>potwierdzamy, że zostały one poprawnie otrzymane</b>.
</p>
<p>
Materiały zostały przekazane do działu produkcji w celu weryfikacji mocowań oraz linii podłogi.<br>
Na ich podstawie realizacja Państwa zamówienia jest kontynuowana.
</p>
<p>
W razie potrzeby dodatkowych informacji skontaktujemy się z Państwem bezpośrednio. <br>
Na ten moment nie są wymagane żadne dalsze działania z Państwa strony.
</p>
<p>
Dziękujemy za współpracę i cierpliwość.
</p>
<p>
Pozdrawiamy serdecznie<br>
<b>Zespół EVAMATS</b>
</p>
```
