# ASP.Net Framework for Blog quotes

Aplikacija je blog za citate, sa slikom i kratkim tekstom, podeljen po autorima i kategorijama.
Arhitektura ima slojeve Api, Domain, Application, Implementation, DataAcces EF
Baza podataka se radi iz koda (code firtst pristup). Dijagram baze u prilogu

Nakon pokretanja aplikacije gadjati rutu /api/test radi upisa pocetnih podataka

Autorizacija se vrsi preko JWT tokena, i svaki korisnik ima svoj slucaj koriscenja (Tabela UserUseCases)

Neautorizovani korisnici mogu samo da se registruju,gde dobijaju i mejl, i mogu da gledaju citate
Autorizovani mogu da prave citate, ostavljaju komentare i ocene
Administrator moze da vrsi CRUD operacije nad tabelama Category, Author, Quote, moze da pregleda Logove 
slucaja koriscenja, kao i da vrsi pretragu. Uradjena je paginacija za sve prikaze. Validacija se vrsi pomocu fluent validatora.

Aplikacija ima Swagger za testiranje
