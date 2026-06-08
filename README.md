# 🚀 ERGO Hestia Pricing Team - Recruitment Landing Page

> **⚠️ DISCLAIMER / UWAGA:** Niniejszy projekt ma charakter wyłącznie koncepcyjny i prototypowy. Został stworzony jako wizja/projekt landing page'a i nie jest oficjalną, produkcyjną stroną internetową firmy ERGO Hestia. Wszelkie logotypy, nazwy własne firm i instytucji użyte w projekcie należą do ich prawnych właścicieli i zostały wykorzystane wyłącznie w celach prezentacyjnych.

## 📖 O projekcie

Projekt nowoczesnego, w pełni responsywnego Landing Page'a zaprojektowanego dla Biura Pricingu. Głównym celem strony jest przyciągnięcie talentów z obszaru Data Science, Inżynierii Danych oraz Analizy Pricingowej poprzez jasne zaprezentowanie kultury pracy, stosowanych technologii oraz konkretnych ofert pracy.

Interfejs został zaprojektowany z naciskiem na minimalizm, czytelność oraz nowoczesne trendy UI, co ma odzwierciedlać zaawansowany technologicznie charakter pracy w dziale analitycznym.

## ✨ Główne cechy projektu

* **Styl Glassmorphism:** Estetyczne, "szklane" kafelki z efektem rozmycia tła (backdrop-filter), nadające stronie lekki i nowoczesny wygląd.
* **Responsywność (Mobile-First):** Płynne dostosowanie układu do ekranów smartfonów, tabletów i monitorów szerokoekranowych (m.in. dynamiczna siatka CSS Grid zmieniająca układ kafelków z benefitami z 2 na 5 kolumn).
* **Interaktywny Slider Horyzontalny:** Sekcja "Czym się zajmujemy" zaimplementowana w formie przewijanego w poziomie paska (z obsługą touch-scroll na urządzeniach mobilnych oraz przyciskami nawigacyjnymi na desktopie).
* **Nieskończona animacja CSS (Marquee):** Płynnie przesuwający się pasek logotypów prezentujący różnorodne zewnętrzne źródła danych.
* **Architektura Zero-Dependency:** Strona została zbudowana w oparciu o czysty kod (Vanilla), bez użycia ciężkich frameworków typu Bootstrap, Tailwind czy zewnętrznych bibliotek JavaScript, co gwarantuje błyskawiczne ładowanie.

## 🛠️ Wykorzystane technologie

* **HTML5** (Semantyczna struktura, tagi `<details>` do natywnej obsługi FAQ i rozwijanych ogłoszeń)
* **CSS3** (Flexbox, CSS Grid, Zmienne CSS, Animacje `@keyframes`, Media Queries)
* **JavaScript (Vanilla)** (Lekki skrypt wspomagający płynne przewijanie slidera)

## 📝 Jak dodać nową ofertę pracy?

Strona została zbudowana modułowo. Aby dodać nową rekrutację, nie musisz zmieniać plików CSS. Wystarczy, że skopiujesz gotowy blok HTML i podmienisz w nim treści.

1. Otwórz plik `index.html`.
2. Znajdź sekcję opisaną komentarzem `<!-- OFERTY PRACY -->` (okolice 260. linijki kodu).
3. Odszukaj kontener `<div class="roles-grid">`.
4. Skopiuj poniższy szablon i wklej go wewnątrz tego kontenera (najlepiej tuż nad kartą "Aplikacja Spontaniczna"):

```html
<!-- KARTA OFERTY: Wpisz nazwę stanowiska -->
<div class="glass-card role-card">
    <div class="role-header">
        <div>
            <span class="role-badge">Nowa oferta</span>
            <h3>Tytuł Stanowiska (np. Data Scientist)</h3>
            <p class="role-location">📍 Lokalizacja (np. Sopot - Hybrydowo)</p>
        </div>
    </div>

    <!-- Tagi technologiczne -->
    <div class="role-tags">
        <span class="tag python">Python</span>
        <span class="tag sql">SQL</span>
        <span class="tag">Inna Technologia</span>
    </div>

    <!-- Rozwijane szczegóły -->
    <details class="role-details">
        <summary>Pokaż szczegóły ogłoszenia</summary>
        <div class="role-details-content">
            
            <h4>Twój zakres obowiązków:</h4>
            <ul>
                <li>Pierwszy obowiązek</li>
                <li>Drugi obowiązek</li>
            </ul>

            <h4>Nasze wymagania:</h4>
            <ul>
                <li>Pierwsze wymóg</li>
                <li>Drugi wymóg</li>
            </ul>

        </div>
    </details>

    <!-- Link do formularza w systemie eRecruiter -->
    <div class="role-footer">
        <a href="TUTAJ_WKLEJ_LINK" target="_blank" class="btn primary full-width">Aplikuj na to stanowisko</a>
    </div>
</div>
```

## 🚀 Jak uruchomić projekt lokalnie?

Projekt nie wymaga instalacji żadnego środowiska serwerowego (Node.js, npm itp.). Aby go uruchomić:

1. Pobierz lub sklonuj to repozytorium na swój dysk:
   ```bash
   git clone [https://github.com/mzntk/ergo-hestia-pricing-landing.git](https://github.com/mzntk/ergo-hestia-pricing-landing.git)
