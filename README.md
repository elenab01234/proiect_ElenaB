#### Proiect Manual Testing – SauceDemo

#### Descriere Proiect

Acest proiect reprezinta o activitate de testare manuala realizata pentru aplicatia web SauceDemo. (https://www.saucedemo.com/)

Scopul proiectului a fost verificarea functionalitatilor principale ale aplicatiei prin proiectarea, executarea si documentarea cazurilor de testare pentru fluxurile critice ale utilizatorului. Au fost executate 32 de cazuri de testare pentru utilizatorii `standard_user` si `error_user`, fiind validate fluxurile de autentificare, gestionare produse, cos de cumparaturi si checkout.

#### Mediu de Testare

| Componenta         | Detalii                   |
| ------------------ | ------------------------- |
| Aplicatie          | SauceDemo                 |
| Browser            | Google Chrome             |
| Tip testare        | Testare manuala           |
| Tehnica de testare | Testare functionala       |
| Sistem de operare  | Windows                   |
| Conturi utilizate  | standard_user, error_user |

#### Obiectivele Testarii

* Validarea functionalitatilor principale ale aplicatiei
* Verificarea mesajelor de eroare si validarilor
* Testarea fluxului complet de cumparare
* Verificarea comportamentului cosului de cumparaturi
* Identificarea defectelor functionale
* Validarea experientei utilizatorului

#### Aria de Testare

Testarea a fost realizata pentru urmatoarele module:

* Login Interface
* Products Page
* Shopping Cart
* Single Product Page
* Checkout Information
* Checkout Overview
* Checkout Complete
  
---
#### Scenarii de Testare Executate

Login Interface:

* Login cu username si parola valida
* Login cu parola invalida
* Login cu username invalid
* Validare camp Username gol
* Validare camp Password gol

Products Page:

* Filtrare produse A-Z
* Filtrare produse Z-A
* Filtrare produse dupa pret crescator
* Filtrare produse dupa pret descrescator
* Adaugare produs in cos
* Eliminare produs din cos
* Adaugare numar maxim de produse in cos
* Eliminare numar maxim de produse din cos
* Logout din meniu

Shopping Cart:

* Continuare cumparaturi
* Verificarea actualizarii numarului de produse
* Checkout cu produse
* Checkout cu cos gol

Single Product Page:

* Navigare inapoi catre pagina de produse
* Adaugare produs in cos
* Eliminare produs din cos
* Functionalitate All Items

Checkout Information:

* Validare campuri obligatorii
* Continuare cu date valide
* Anulare checkout

Checkout Overview:

* Verificare informatii comanda
* Finalizare comanda
* Anulare comanda

---
#### Rezumat Executie Teste – standard_user

| Status  | Numar Teste |
| ------- | ----------- |
| Pass    | 30          |
| Fail    | 2           |
| Blocked | 0           |

#### Defecte Identificate – standard_user

| BUG ID | Descriere                                                 |
| ------ | --------------------------------------------------------- |
| BUG-01 | Informatiile de livrare lipsesc in Checkout Overview Page |
| BUG-02 | Aplicatia permite checkout cu cos gol                     |

---

#### Rezumat Executie Teste – error_user

| Status  | Numar Teste |
| ------- | ----------- |
| Pass    | 18          |
| Fail    | 9           |
| Blocked | 5           |

#### Defecte Identificate – error_user

| BUG ID | Descriere                                                 |
| ------ | --------------------------------------------------------- |
| BUG-02 | Aplicatia permite checkout cu cos gol                     |
| BUG-03 | Functionalitatea de sortare produse este defecta          |
| BUG-04 | Functionalitatea Add to cart nu actualizeaza corect cosul |
| BUG-05 | Nu toate produsele pot fi adaugate in cos                 |
| BUG-06 | Functionalitatea Remove nu functioneaza corect            |
| BUG-07 | Add/Remove din Single Product Page nu functioneaza        |
| BUG-08 | Campul Last Name nu permite introducerea datelor          |
| BUG-09 | Checkout permite continuarea fara Last Name               |
| BUG-10 | Finish nu redirectioneaza catre Finish Page               |

---
#### Instrumente Utilizate

* Google Sheets/ Docs
* GitHub Projects (task management)

---
#### Concluzie

Rezultatele obtinute au evidentiat atat functionalitati stabile, cat si defecte functionale importante in modulele Products Page si Checkout, in special pentru utilizatorul `error_user`.

Proiectul demonstreaza capacitatea de:

* creare a cazurilor de testare
* executare manuala a testelor
* identificare si raportare defecte
* analiza rezultatelor testarii
* documentare QA pentru aplicatii web

 ---


