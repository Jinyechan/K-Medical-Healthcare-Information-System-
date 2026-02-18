# K-MEDICAL  
### Data-Driven Healthcare Information Platform  

---

## Project Overview

K-MEDICAL ist eine datengetriebene Full-Stack-Webanwendung zur Aggregation, Visualisierung und Interaktion mit medizinischen Infrastrukturdaten in Südkorea.

Die Plattform integriert:

- Universitätskliniken-Metadaten  
- Geospatiale Visualisierung (Kakao Maps SDK)  
- REST-basierte medizinische Gerätesuche  
- Krebsinzidenz-Datenanalyse (Chart.js)  
- Authentifiziertes Review-System  
- Versicherungs- und Reservierungsinformationen  

Das Projekt demonstriert Full-Stack-Integration mit Flask, REST APIs, asynchroner Datenverarbeitung und modularer UI-Architektur.

---

## Tech Stack

### Frontend
- HTML5 (Jinja2 Templating)
- CSS3
- Bootstrap 5
- JavaScript (ES6+)
- jQuery (AJAX)
- Chart.js
- Kakao Maps SDK
- AOS (Scroll Animation)

### Backend
- Python
- Flask
- Jinja2
- RESTful API Design
- Session-basierte Authentifizierung
- MVC-orientierte Struktur

---

## Project Structure

pycache/
static/
│ ├── fonts/
│ └── images/
templates/
│ ├── index.html
│ ├── login.html
│ └── Interactive-1.interactive.ipynb
README.md
app.py
models.py


---

## System Architecture

### Application Layer (app.py)

- Routing
- REST-Endpunkte
- Session-Handling
- JSON-Responses
- Integration der Datenmodelle

### Data Layer (models.py)

- Datenbankmodelle
- ORM-Strukturen
- Persistenzlogik
- Relationen (User ↔ Reviews)

### Presentation Layer (templates/)

- Single-Page-Struktur mit Scroll-Navigation
- Kartenmodul
- Statistik-Dashboard
- Gerätesuche
- Authentifiziertes Review-System

---

## Core Functional Modules

### 1. Hospital Directory

- Strukturierte Darstellung führender Universitätskliniken
- Kartenbasierte Visualisierung
- Externe Weiterleitungen
- Responsive Card-Layout

### 2. Geospatial Search

Integration von Kakao Maps:

- Marker Rendering
- InfoWindow Events
- Geocoder-basierte Regionssuche
- Dynamische Viewport-Anpassung

### 3. Disease-Based Medical Device Search

REST Endpoint:

GET /api/search?disease=<query>

- Asynchrone Datenabfrage
- JSON-basierte Antwort
- Dynamisches Rendering
- Fehlerbehandlung

### 4. Cancer Statistics Dashboard

REST Endpunkte:

- GET /api/cancer/gender  
- GET /api/cancer/age  
- GET /api/cancer/gender-specific  

Features:

- Chart.js Visualisierung
- Pagination-Logik
- Dynamische Dataset-Aktualisierung
- Periodische Aktualisierung

### 5. Authenticated Review System

REST Endpunkte:

- GET /get_user  
- POST /review  
- GET /review?page=<n>  

- 5-Sterne Bewertungssystem
- Session-Validierung
- Server-side Pagination
- Dynamisches Nachladen

---

## Engineering Competencies

- Full-Stack Web Development
- REST API Design & Consumption
- Third-Party SDK Integration
- Asynchronous Programming
- Data Visualization
- Session-based Authentication
- Modular UI Architecture
- Separation of Concerns

---

## Deployment (Development)

1. Repository klonen  
2. Virtuelle Python-Umgebung erstellen  
3. Abhängigkeiten installieren  
4. Flask-Server starten  

Produktivumgebung empfohlen mit:
- Gunicorn
- Nginx
- Docker
- PostgreSQL

---

## Professional Relevance

Dieses Projekt demonstriert:

- Architekturverständnis im Client-Server-Kontext  
- Skalierbare Webapplikationsstruktur  
- Datengetriebene UI-Implementierung  
- Authentifizierungs- und Zustandsmanagement  
- Erweiterbare REST-basierte Systemarchitektur  
