
# 418	Wysyłanie e-maili- automatyzacja
## Wyślij wiadomość e-mail do klienta
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

# 442	Wysyłanie email po stworzeniu e-paragona
# 446	Wysyłanie email po stworzeniu faktury
# 498	Wysłanie komunikacji "Czekam na opłatę"
# 550	Wezwanie przedsądowe
# 718	Workflou dla etapu "Informacja zwrotna"
# 766	Akceptacja kompletów: Potwierdzenie otrzymania zdjęć
