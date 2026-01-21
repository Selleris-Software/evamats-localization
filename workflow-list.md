
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
# 446	Wysyłanie email po stworzeniu faktury
# 498	Wysłanie komunikacji "Czekam na opłatę"
# 550	Wezwanie przedsądowe
# 718	Workflou dla etapu "Informacja zwrotna"
# 766	Akceptacja kompletów: Potwierdzenie otrzymania zdjęć
