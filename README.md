# Schritt-für-Schritt-Einführung in das Web-Framework [Symfony]

**Der Kurs ist hier online verfügbar: [https://stahe.github.io/de-symfony-sept-2026/](https://stahe.github.io/de-symfony-sept-2026/)**

## Autor

Der Kurs und sein gesamter Code wurden von **Claude**, der KI von Anthropic, als **alleinigem Autor** im Auftrag von Serge Tahé geschrieben (September 2026).

## Überblick

Dieser Kurs bietet eine Schritt-für-Schritt-Anleitung zum Aufbau einer MVC-Webanwendung mit dem Framework **Symfony 8.1** und der Sprache **PHP 8.4**. Die HTML-Seiten werden serverseitig mit **Twig**-Views erzeugt, ohne ein browserseitiges JavaScript-Framework. Der Datenzugriff erfolgt über das ORM **Doctrine**.

Er überträgt den Kurs [Schritt-für-Schritt-Einführung in das Web-Framework [Laravel]](https://stahe.github.io/de-laravel-sept-2026/) – der seinerseits auf den Kursen zu [Flask](https://stahe.github.io/de-flask-sept-2026/), [Spring MVC](https://stahe.github.io/de-springmvc-sept-2026/), [ASP.NET Core MVC](https://stahe.github.io/de-aspnetcoremvc-sept-2026/) und [NestJS](https://stahe.github.io/de-nestjs-html-sept-2026/) beruht. Die Beispiele haben dieselben Nummern und behandeln dieselben Themen: Die Frameworks lassen sich Beispiel für Beispiel vergleichen.

## Inhalt

| Kapitel | Themen | Beispiele |
|---|---|---|
| Actions, Routing, Antworten | Routen (`#[Route]`), Controller, Antworten, Weiterleitungen, Service-Container | 01 bis 06 |
| Das Action-Modell | Request-Parameter, Argument Resolver, Validierungsconstraints, POST-Requests | 07–12 |
| Die View und ihr Modell | Twig, Templates, Makros, Erweiterungen, Form-Komponente, Validierung, Post/Redirect/Get, CSRF-Schutz | 13–21 |
| Internationalisierung | eine Anwendung auf Französisch und Englisch (YAML-Wörterbücher, ICU-Nachrichten) | 22 |
| Datenbereiche | Request, Session, Cache, Cookies | 23 |
| Der Lebenszyklus einer Anfrage | Kernel-Events, Listener, Argument Resolver, Fehlerseiten | 24 |
| Authentifizierung und Autorisierung | Firewall, JWT-Authenticator in einem Cookie, Rollen, CAPTCHA, Rate Limiting | 25–27 |
| Schichtenarchitektur | Web / Geschäftslogik / DAO mit Doctrine und MySQL | 28 |
| Fallstudie | **RdvMedecins**, eine Anwendung zur Terminplanung in einer Arztpraxis, Datei für Datei erläutert | - |

Die Fallstudie `rdvmedecins2-symfony` verwaltet drei Rollen (Administrator, Ärzte, Patienten): Kalender, Buchungen, Arzt- und Kundenverwaltung, durch CAPTCHA geschützte Kontoerstellung und eine französisch-englische Oberfläche. Sie verwendet dieselbe Datenbank `dbrdvmedecins2` wie die anderen Versionen der Anwendung.

## Voraussetzungen

- PHP 8.4 oder neuer (Erweiterungen `intl`, `mbstring`, `openssl`, `pdo_mysql`);
- Composer 2;
- MySQL 8 oder MariaDB (Laragon unter Windows);
- Visual Studio Code mit den Erweiterungen PHP Intelephense, Twig Language 2 und YAML;
- curl.

Der Quellcode kann von der Kurswebsite heruntergeladen werden. Die `vendor`-Ordner sind dort nicht enthalten: `composer install` erstellt sie – einen im Ordner `exemples` und einen im Ordner `rdvmedecins2-symfony`.
