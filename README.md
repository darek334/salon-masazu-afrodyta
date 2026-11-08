# Salon Masażu

**System internetowy do zarządzania salonem masażu**

Projekt zespołowy realizowany w ramach zajęć na uczelni Vistula.

## O projekcie

Celem projektu jest opracowanie aplikacji internetowej wspierającej zarządzanie działalnością salonu masażu.

System będzie umożliwiał gromadzenie, przetwarzanie i udostępnianie informacji związanych z funkcjonowaniem salonu, w szczególności dotyczących klientów, pracowników, oferowanych usług oraz rezerwacji.

Aplikacja zostanie zaprojektowana jako rozwiązanie webowe, dostępne za pośrednictwem przeglądarki internetowej, bez konieczności instalowania dedykowanego oprogramowania na urządzeniu użytkownika.

## Architektura techniczna

Przyjęto koncepcję architektury trójwarstwowej (*Three-Tier Architecture*), obejmującej:

| Warstwa | Technologie |
|---|---|
| Presentation Layer – warstwa prezentacji | HTML, CSS, JavaScript |
| Application Layer – warstwa logiki aplikacji | PHP |
| Data Layer – warstwa danych | MySQL |

Komunikacja pomiędzy warstwami będzie realizowana z wykorzystaniem:

- **HTTPS i JSON** – komunikacja pomiędzy przeglądarką internetową a serwerem aplikacji.
- **PDO i SQL** – komunikacja pomiędzy aplikacją PHP a bazą danych MySQL.

Szczegółowe założenia architektoniczne są dokumentowane w katalogu `docs`.

## Wykorzystywane technologie

- HTML5
- CSS3
- JavaScript
- PHP
- MySQL
- SQL
- PDO
- Git
- GitHub

## Struktura dokumentacji - początkowe założenia

```text
salon-masazu/
│
├── frontend/                     # Warstwa prezentacji główna strona aplikacji - GUI
│   ├── css/
│   ├── html/
│   ├── js/
│   ├── images/
│   └── php/                      # index.php
│
├── backend/                      # Warstwa pośrednia - endpointy
│   ├── endpoint_schema/          # podstawowy schemat struktury katalogów endpointa
│   │   ├── php/                    # index.php
│   │.................            # następne endpointy
│   └── classes/
│
├── database/                     # Warstwa danych - baza danych
│   ├── table_schema/             # podstawowy schemat struktury katalogów definiujących tabele
│   ├.................            # następna tabela, każda tabela ma mieć swój oddzielny katalog. Triggery itp do tego samego katalogu
│
├── docs/                         # Folder na dokumentacje projektu
│   └── main_architecture.md      # Podstawowe założenia
│
├── .gitignore
└── README.md
```

*Struktura katalogów ma charakter wstępny i będzie rozwijana wraz z postępem prac.*

## Organizacja pracy

Do zarządzania zadaniami i monitorowania postępu prac wykorzystywana jest platforma Jira.

GitHub służy do przechowywania kodu źródłowego, dokumentacji technicznej oraz historii zmian w projekcie.

## Status projektu

Projekt znajduje się na etapie opracowywania założeń architektonicznych i planowania prac.

## Zespół projektowy

Skład zespołu oraz zakres odpowiedzialności poszczególnych członków zostaną uzupełnione w trakcie organizacji projektu.
