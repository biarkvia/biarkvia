<h1 align="center">Hi, I'm Viachaslau Biarko 👋</h1>

<h3 align="center">Backend Developer · Kotlin for Android &amp; JVM · Systems Programming · Windows &amp; Linux Administration</h3>

<p align="center">Prague, Czechia · PHP · Kotlin · Ruby on Rails · SQL · C++ · Linux</p>

<p align="center">
  <a href="mailto:slava.biarko@gmail.com">Email</a> ·
  <a href="https://www.linkedin.com/in/slavassse/">LinkedIn</a> ·
  <a href="https://biarkvia.github.io/voltar-auto/">VOLTAR AUTO · živá ukázka</a>
</p>

---

## About Me

At **OXIT**, I developed internal CRM software for inventory, pricing, invoicing and transport using PHP, Nette, Doctrine ORM and MySQL/MariaDB. I built stock movement tracking and a tool to reconstruct missing warehouse history. I also implemented multi-currency pricing with quantity discounts, optimized SQL for financial reports and integrated Microsoft 365 services through REST APIs.

I work in systems administration at **Charles University**, supporting Windows and Linux servers, Active Directory and HP/Aruba networks. I use PowerShell and Bash to troubleshoot server and network issues. During a research internship at **Axis FF**, I compared standards for representing physical assets in digital twins.

My public projects cover business software, Android apps that work offline, and data structures. Below are examples in PHP, Kotlin, Ruby and C++. My Windows–Linux Office Lab shows how I use PowerShell and Ansible to manage access across a Windows domain and an Ubuntu file server.

---

## Core Technologies

### Backend & databases

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![Nette](https://img.shields.io/badge/Nette-3484D2?style=for-the-badge)
![Symfony](https://img.shields.io/badge/Symfony-000000?style=for-the-badge&logo=symfony&logoColor=white)
![Ruby on Rails](https://img.shields.io/badge/Ruby_on_Rails-D30001?style=for-the-badge&logo=rubyonrails&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

### Kotlin, Android & JVM

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack_Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white)
![Room](https://img.shields.io/badge/Room-386A20?style=for-the-badge)
![Ktor](https://img.shields.io/badge/Ktor-6558D3?style=for-the-badge)
![Compose Desktop](https://img.shields.io/badge/Compose_Desktop-35495E?style=for-the-badge)

### Systems & tooling

![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![NGINX](https://img.shields.io/badge/NGINX-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

### Infrastructure & automation

- **Windows Server & Hyper-V** · Active Directory Domain Services, DNS, Group Policy drive mappings and PowerShell provisioning.
- **Ubuntu & Ansible** · Samba domain membership with Winbind, signed SMB and department shares with POSIX ACLs.
- **Backup & monitoring** · Scheduled backups with systemd timers, Zabbix alerts for overdue copies and recovery checks from Windows 11.

---

## Featured Projects

### Windows–Linux Office Lab · Domain access and file server recovery

I built a four-VM office network on Hyper-V and tested it from an employee’s Windows 11 desktop. When I moved the account from Finance to Sales, Group Policy mapped the same `S:` drive to Sales. I verified that the employee could write there and that opening the old Finance share directly returned access denied.

In a recovery drill, I restored the Samba file server on a clean Ubuntu VM. **12 minutes 15 seconds** after I declared the outage, the employee could open the original path again. The restored file matched its SHA-256 checksum, and the department restrictions still held.

[View repository](https://github.com/biarkvia/windows-linux-office-lab) · [Recovery report](https://github.com/biarkvia/windows-linux-office-lab/blob/main/docs/step-8.md)

---

### VOLTAR AUTO · Ukázka webu

Ukázka webu pro fiktivní pražský autoservis VOLTAR AUTO. Prohlédněte si služby a galerii dílny nebo si vyzkoušejte poptávkový formulář bez odesílání údajů.

[Otevřít živou ukázku](https://biarkvia.github.io/voltar-auto/) · [Zdrojový kód](https://github.com/biarkvia/voltar-auto)

---

### Actifity · Sports bookings and event management

I built Actifity for sports organizers and their participants. Participants can filter classes by sport, date or location, book a place and cancel a reservation. Organizers create events and manage participant lists. I tested the booking flow with users in both roles.

**Stack** · PHP, Nette, Doctrine ORM, MySQL, JavaScript, REST APIs, Docker

[View repository](https://github.com/biarkvia/actifity)

---

### Station Directory · Offline Android app

Users can open a station and check each device's status and last contact, even after restarting the app offline. Room keeps the last successful response and distinguishes a station with zero devices from one whose devices have never been downloaded.

The test suite covers the API, database transactions and Compose screens, including a slow response arriving after the user has switched stations. GitHub Actions runs the checks and publishes a signed APK for release tags.

**Stack** · Kotlin, Jetpack Compose, Room, Ktor, Coroutines, Flow, Navigation 3, Firebase Crashlytics

[View repository](https://github.com/biarkvia/station-directory) · [Download the Android release](https://github.com/biarkvia/station-directory/releases/latest)

---

### Renewal Desk · Contract renewal tracking

Contract owners can track notice deadlines, receive reminders and record renewal decisions. Version checks protect concurrent edits, and overlapping background jobs produce a single reminder. Users can also paste a contract excerpt and review suggested dates alongside the wording that supports them.

**Stack** · Ruby on Rails, PostgreSQL, Solid Queue, OpenAI Responses API, Minitest, Docker

[View repository](https://github.com/biarkvia/renewal-desk)

---

### R-Tree · Spatial indexing in Kotlin

I built a file-backed index for multidimensional rectangles. It can find all rectangles intersecting a region or the nearest neighbors to a point. The Compose Desktop app lets you insert data and try both queries. The experiments compare the index with a linear scan as the number of dimensions changes.

**Stack** · Kotlin/JVM, Compose Desktop, binary file I/O, Gradle

[View repository](https://github.com/biarkvia/vwm_r_tree) · [Experiment results](https://github.com/biarkvia/vwm_r_tree/tree/main/experiment_results)

---

### CDN IPv6 routing & NGINX

A C++ router selects a point of presence by matching an EDNS Client Subnet against the most specific IPv6 prefix. A separate NGINX header filter written in C exposes the cache key in a response header for inspection.

**Stack** · C++, C, IPv6, NGINX, LuaJIT FFI, CMake

[View repository](https://github.com/biarkvia/cdn77-infrastructure-tasks)

---

## More Projects

| Project | What you'll find |
| --- | --- |
| [Symfony Shop](https://github.com/biarkvia/symfony-shop) | A PHP storefront with a cart, checkout and EasyAdmin back office. Tests cover order rules and checkout against a simulated payment gateway. |
| [FAVI Partner Order API](https://github.com/biarkvia/favi-api) | A Symfony REST API for accepting partner orders and updating delivery dates, with distinct handlers for each operation. |
| [FirmaCheck](https://github.com/biarkvia/firmacheck) | A TypeScript and Next.js app for looking up Czech companies by IČO in the ARES registry. It caches results in Turso, maps addresses and exports saved companies to CSV. |
| [HR & Timesheet Platform](https://github.com/biarkvia/hr-and-timesheet-platform) | An early-stage Ktor backend with PostgreSQL migrations for employees, timesheets and approval history. Its readiness endpoint checks the database connection. |
| [C++ networking & systems exercises](https://github.com/biarkvia/biarkvia_repository) | A TCP server that forks a process per client, alongside separate threading and synchronization exercises, algorithms, and experiments with MongoDB and the Elastic Stack. |

---

## Education

**BSc in Informatics · Web Engineering**  
Faculty of Information Technology, Czech Technical University in Prague · 2026

---

<p align="center">Explore my pinned repositories below ↓</p>
