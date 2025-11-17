# Brainstorming Session Results

**Session Date:** 2025-11-17
**Facilitator:** Business Analyst Mary
**Participant:** Mariusz

## Session Start

**Selected Focus Areas:**
1. Problemy użytkowników i pain pointy - Jakie wyzwania naprawdę rozwiązujemy?
2. Innowacyjne funkcje - AI symptom checker, personalizacja, marketplace
3. Podejścia techniczne - Flutter, multi-tenancy, FHIR/HL7, offline-first
7. Ryzyka techniczne - Security, compliance (HIPAA/GDPR), integracje
8. Metryki sukcesu - KPI dla każdej grupy użytkowników

**Approach:** Progressive Flow - 4 komplementarne techniki

**Planned Journey:**
1. Mind Mapping (15-20 min) - Divergent exploration, visual mapping
2. What If Scenarios (15-20 min) - Creative expansion, radical possibilities
3. Six Thinking Hats (20-25 min) - Analytical depth, multi-perspective analysis
4. Assumption Reversal (15 min) - Convergent synthesis, challenge assumptions

**Estimated Duration:** 65-80 minutes

## Executive Summary

**Topic:** YourMedic - Wieloplatformowa aplikacja medyczna łącząca pacjentów, lekarzy i kliniki

**Session Goals:**
- Zidentyfikować kluczowe problemy użytkowników (pacjenci, lekarze, kliniki)
- Zbadać innowacyjne funkcje (AI symptom checker, marketplace, personalizacja)
- Przeanalizować podejścia techniczne (Flutter cross-platform, FHIR/HL7, offline-first)
- Zidentyfikować ryzyka techniczne (security, HIPAA/GDPR compliance, integracje EHR)
- Zdefiniować metryki sukcesu dla każdej grupy użytkowników

**Techniques Used:** {{techniques_list}}

**Total Ideas Generated:** {{total_ideas}}

### Key Themes Identified:

{{key_themes}}

## Technique Sessions

### Technique 1: Mind Mapping (Structured, 15-20 min)

**Central Concept:** YourMedic - Wieloplatformowa aplikacja medyczna

#### Branch 1: Problemy Użytkowników i Pain Pointy

**👥 PACJENCI:**

**Główne bóle/frustracje:**
- **Brak jasnej ścieżki pomocy** - nie wiedzą, do jakiego specjalisty iść, co zrobić z objawami, czy to pilne
- **Długi czas oczekiwania** - NFZ 6-9 miesięcy, prywatnie obdzwonienie kilku miejsc
- **Rozsypane informacje o zdrowiu** - wyniki z labu w mailu, skierowania na kartce, zalecenia w SMS-ie, e-recepty w innym systemie
- **Zero "centrum sterowania zdrowiem"**

**Trudności z umawianiem/komunikacją:**
- Umawianie wymaga dzwonienia w godzinach pracy (konflikt z własną pracą)
- Strony www/portale placówek mało intuicyjne - brak jasnej informacji o cenach, czasie wizyty, dostępności
- Brak prostego kanału do krótkich pytań - trzeba umawiać pełną wizytę dla jednego pytania
- Brak transparentności - pacjent nie widzi wolnych terminów i realnych kosztów

**Gdzie tracą czas/pieniądze:**
- Szukanie lekarza - fora, grupy FB, kilka portali, porównywanie opinii (godziny przepalone)
- Powtarzanie badań - bo inny lekarz/klinika nie widzi wyników
- Niepotrzebne wizyty - mogłyby być załatwione czatem/teleporadą ("czy przedłużyć antybiotyk?")
- Niepojawianie się - brak przypomnienia = zapomniana wizyta = utrata zaliczki

**Jak YourMedic adresuje:**
- ✅ Jeden profil zdrowotny 360° (historia chorób, wyniki, leki, alergie, wizyty)
- ✅ AI Symptom Checker (pomaga zdecydować do kogo iść i czy pilne)
- ✅ Jeden panel rezerwacji (terminy różnych lekarzy/klinik + płatność online)
- ✅ Czat + follow-up (proste pytania, opieka po wizycie, przypomnienia)

---

**🩺 LEKARZE:**

**Główne bóle/frustracje:**
- **Biurokracja zjada czas** - wypełnianie dokumentacji, przepisywanie danych w kilku systemach, ręczne pisanie zaleceń
- **Chaos w grafiku** - telefony, odwołania, zapomniane wizyty, brak centralnego systemu real-time
- **Brak pełnego obrazu pacjenta** - wyniki z różnych miejsc, brak dostępu do historii, pacjent "przynosi segregator"
- **Wypalenie** - dużo powtarzalnych czynności, mało realnej medycyny

**Trudności z umawianiem/komunikacją:**
- Część wizyt przez recepcję, część przez portale, część przez prywatny telefon - brak jednego źródła prawdy
- Brak prostego narzędzia do bezpiecznego czatu (wszystko na SMS/WhatsApp - nie idealne)
- Brak możliwości szybkiego follow-upu ("jak się czujesz po zmianie leku?")

**Gdzie tracą czas/pieniądze:**
- Papierologia - opisy wizyt, wypisy, zalecenia (wszystko ręcznie lub w Wordzie)
- No-show pacjentów - brak automatycznych przypomnień i łatwej listy rezerwowej = puste okienka
- Rozproszone narzędzia - osobno kalendarz, osobno fakturowanie, osobno portal do teleporad

**Jak YourMedic adresuje:**
- ✅ Jedno miejsce: kalendarz, pacjenci, dokumentacja, komunikacja
- ✅ AI-asystent automatycznie tworzy szkic opisu wizyty i zaleceń (lekarz tylko akceptuje/poprawia)
- ✅ Automatyczne przypomnienia + lista oczekujących minimalizują puste okienka
- ✅ Bezpieczny czat i wideokonsultacje obsługują część spraw bez wizyt w gabinecie

---

**🏥 KLINIKI/PLACÓWKI:**

**Główne bóle/frustracje:**
- **Trudność w ogarnięciu grafiku całego zespołu** - lekarze na etacie, kontraktowi, wynajmujący gabinety, rotacje, zmiany
- **Brak integracji systemów** - osobno rejestracja, osobno rozliczenia, osobno dokumentacja medyczna
- **Nieprzewidywalne obłożenie** - są dni/szczeliny puste i takie zapchane
- **Problem z anulacjami i no-show** - brak automatycznego mechanizmu "łatania dziur"

**Trudności z umawianiem/komunikacją:**
- Rejestracja na telefon + Excel + kartka
- Trudno mieć aktualny podgląd dostępności wszystkich lekarzy w jednym miejscu
- Brak prostych narzędzi do masowego informowania pacjentów (zmiana godzin, nowy lekarz, odwołanie)

**Gdzie tracą czas/pieniądze:**
- Ręczne zarządzanie grafikiem, kopiowanie danych między systemami, poprawianie błędów
- Niewykorzystane sloty - pacjent nie przychodzi, brak systemu automatycznego podstawienia z listy oczekujących
- Słaby marketing - trudność z mierzeniem skąd przychodzą pacjenci, co działa

**Jak YourMedic adresuje:**
- ✅ Centralny panel: zarządzanie lekarzami, grafikiem, salami, obłożeniem
- ✅ Automatyczna obsługa przypomnień, anulacji, listy rezerwowej (mniej przepadających terminów)
- ✅ Integracja z płatnościami i fakturowaniem upraszcza rozliczenia
- ✅ Moduł raportowy: analiza obłożenia, przychodów, źródeł pacjentów

**💎 KEY INSIGHT:**
> **Pacjent** przestaje błądzić po systemie - ma jedną aplikację do objawów, lekarzy, wyników i płatności.
> **Lekarz** przestaje tonąć w papierologii - ma smart kalendarz, AI-asystenta dokumentacji i bezpieczną komunikację.
> **Klinika** przestaje zarządzać chaosem - ma jeden panel do grafiku, zasobów, pacjentów i pieniędzy.
> **YourMedic łączy te trzy światy w jednym ekosystemie.**

---

#### Branch 2: Innowacyjne Funkcje - Jak rozwiązujemy problemy

**🤖 AI SYMPTOM CHECKER - Inteligentny Triage**

**3 Poziomy rozwoju:**

**Poziom 1: Podstawowy MVP (0-6 miesięcy)**
- Wywiad chorobowy krok po kroku (chatbot style)
- Model ciała 3D do wskazania miejsca bólu
- Kalendarz + intensywność (skala 1-10)
- Output: 3-5 możliwych przyczyn z % prawdopodobieństwa
- Alarm level: 🟢 może poczekać / 🟡 wizyta w 48h / 🔴 SOR natychmiast
- Rekomendacja specjalisty konkretnego

**Poziom 2: Zaawansowany (3-6 miesięcy)**
- Pytania kontekstowe (AI zna historię pacjenta: alergie, choroby, leki)
- Analiza zdjęć (wysypka, rana - basic dermatology recognition)
- Sugestie badań przed wizytą
- Edukacja (wideo/artykuł wyjaśniający)

**Poziom 3: Pro (rok+)**
- Multimodal AI (głos + tekst + obraz + wearables)
- Predykcja zdrowotna ("Ryzyko cukrzycy: 15%")
- Integracja z EHR (korelacja z wynikami laboratoryjnymi)

**⚠️ KRYTYCZNE GRANICE:**
- ❌ NIGDY definitywna diagnoza - zawsze "możliwe przyczyny"
- ✅ Zawsze disclaimer: "To nie zastępuje wizyty u lekarza"
- 🚨 Red flags auto-pilot: Objawy zagrożenia życia → natychmiast SOR
- 📜 Certyfikacja: EU wyrób medyczny klasy IIa (jeśli "wspomaga diagnostykę")
- 🎯 **Złoty środek:** AI jako triage tool, NIE narzędzie diagnostyczne (unika regulacji)
- 💬 Marketing: "Inteligentny asystent zdrowotny" zamiast "AI doktor"

---

**🏪 MARKETPLACE LEKARZY - Uber dla Zdrowia**

**A) Profil lekarza = Wizytówka 360°**
- Zdjęcie, bio, certyfikaty (nr PWZ/GMC ZWERYFIKOWANY!)
- Specjalizacje szczegółowe ("kardiolog dziecięcy", "kardiolog sportowy")
- Języki, lokalizacje (multi-site)
- **Cennik transparentny:**
  - Konsultacja online: 150 PLN (30 min)
  - Wizyta osobista: 200 PLN
  - Badanie USG: 300 PLN
- Dostępność real-time (4 tygodnie + badge "Dziś wolne o 18:00")

**B) System rankingowy - 3 wymiary:**

**1. Oceny pacjentów (rozdzielone kategorie):**
- Profesjonalizm ⭐⭐⭐⭐⭐
- Komunikacja ⭐⭐⭐⭐☆
- Punktualność ⭐⭐⭐⭐⭐
- Stosunek jakości do ceny ⭐⭐⭐☆☆

**2. Algorytmiczny score (ukryty, wpływa na ranking):**
- % potwierdzeń vs. odwołania przez lekarza
- Średni czas odpowiedzi w chacie
- Compliance z follow-up
- Wskaźnik "cure rate" (czy pacjenci wracają z tym samym?)

**3. Weryfikacja profesjonalna (badges):**
- ✅ Zweryfikowany specjalista (sprawdzony nr licencji)
- 🏆 Top 10% w specjalizacji
- 📚 Publikacje naukowe
- 🎓 Wykładowca akademicki

**C) Filtry Smart:**
- Standardowe: Miasto, specjalizacja, cena, data
- Smart: "Przyjmuje dzieci/seniorów", języki, "Dostępny dziś/jutro", "NFZ/NHS", "Teleporada możliwa"

**D) Ceny dynamiczne - Model hybrydowy:**
- Bazowa cena = lekarz decyduje
- Dynamic pricing **OPCJONALNIE:**
  - ❌ "Surge pricing" jak Uber - ŹLE w medycynie
  - ✅ "Early bird discount": -20% przy rezerwacji 2 tygodnie wcześniej
  - ✅ "Last minute fill": -15% na jutro (wolny slot)
  - ✅ Package deals: 3 wizyty kontrolne za 500 PLN zamiast 3x200

**E) Prowizja platformy:**
- B2C: 15-20% od wartości wizyty (płaci lekarz)
- Subskrypcja: 99 PLN/miesiąc + 10% prowizji (zamiast 20%)
- Freemium dla klinik: Do 50 wizyt/miesiąc gratis → potem pakiety

---

**🎯 PERSONALIZACJA - Każdy użytkownik inny świat**

**A) DLA PACJENTA:**

**Homepage adaptacyjny:**
- Młoda osoba (18-30): Teleporada, dermatologia, ginekologia
- Rodzic (30-45): Pediatra top widget, szczepienia, ortopeda
- Senior (60+): Kardiolog, diabetolog, wizyty domowe, PROSTSZE UI (większe przyciski)

**Rekomendacje lekarzy:**
- Historia: "Odwiedziłeś 2 ortopedów → może neurochirurg?"
- Lokalizacja: Domyślnie 5 km promień
- Język preferowany: Priorytet anglojęzyczni lekarze

**Smart reminders:**
- "Ostatni raz u dentysty rok temu - czas na kontrolę!"
- "Badania morfologii z marca warto powtórzyć"
- "Za 3 dni kończy się recepta na [lek] - przedłużyć przez teleporadę?"

**B) DLA LEKARZA:**

**Dashboard customizable:**
- Chirurg: "Zabiegi tego tygodnia", "Sala operacyjna", "Follow-up po zabiegach"
- Psycholog: "Cykl terapii pacjenta X - sesja 5/10", "Notatki z poprzednich sesji"
- Dermatolog: "Porównaj zdjęcia znamienia - wizyta 1 vs. 3"

**AI asystent kontekstowy:**
- "Pacjent X ma alergię na penicylinę" - popup przy przepisywaniu
- "Ostatni CRP: 45 mg/L (podwyższony)" - auto-insert do opisu wizyty

**C) DLA KLINIKI:**

**Operational intelligence:**
- "Piątki 16-18: 80% no-shows → zmniejszyć sloty?"
- "Dr Kowalski najwyższy patient satisfaction → więcej godzin?"
- "Sala 3 niewykorzystana środy → dodać fizjoterapię"

**Źródła danych do personalizacji:**
- Demograficzne: Wiek, płeć, lokalizacja
- Historia wizyt: Specjalizacje, częstotliwość, preferencje
- Dane zdrowotne: Choroby przewlekłe, alergie, ryzyko (za zgodą!)
- Behavior tracking: Kliknięcia, wyszukiwania, odwołania
- Wearables: Garmin/Apple Watch → "Puls spoczynkowy rośnie → kardiolog?"

---

**⚕️ FOLLOW-UP SYSTEM - 50% Auto + 50% Human Touch**

**🤖 CO AUTOMATED:**

**Post-wizyta (1h po):**
- SMS: "Jak się czujesz? [Link do ankiety]"
- Auto-zalecenia w PDF (wygenerowane przez lekarza)

**2-3 dni po:**
- Push: "Czy zacząłeś leki? [Tak/Nie/Przypomnij jutro]"
- Jeśli zabieg: "Czy rana się goi? [Pokaż zdjęcie]" → AI ocenia → Escalate jeśli problem

**Tydzień po (zabieg):**
- Email: "Czas na kontrolę - umów się [Link]"

**Chroniczne (np. cukrzyca):**
- Co miesiąc: "Czas zmierzyć HbA1c - laboratorium [Mapa]"
- Co tydzień: "Poziomy cukru? [Wpisz wyniki]" → wykres trendu

**👨‍⚕️ CO HUMAN TOUCH:**

**Lekarz decyduje:**
- Czy follow-up potrzebny (checkbox przy zamykaniu wizyty)
- Kiedy (3 dni / tydzień / miesiąc)
- Czy automated reminder czy osobisty telefon/czat

**Nurse/Asystent kliniczny:**
- Pielęgniarka dzwoni do pacjentów wysokiego ryzyka
- Chatbot eskaluje: "Pacjent: gorączka 39°C po zabiegu" → Alert dla lekarza

**Gamification:**
- "5 wizyt kontrolnych wykonanych - zniżka 10%!"
- "30 dni przyjmowania leków codziennie 🎉"

---

**⌚ INTEGRACJE Z WEARABLES - Od danych do akcji**

**Jakie dane zbierać?**

**Tier 1: Podstawowe (Apple Health, Google Fit):**
- Kroki, kalorie, sen
- Puls spoczynkowy, HRV
- Aktywność (bieganie, siłownia)

**Tier 2: Medyczne (Garmin, Oura, Fitbit):**
- SpO2 (saturacja krwi)
- EKG (Apple Watch/Withings)
- Temperatura ciała (Oura)
- Stres (HRV-based)

**Tier 3: Dedykowane medyczne (API):**
- Glukometr (Freestyle Libre)
- Ciśnieniomierz Bluetooth
- Waga z % tłuszczu (Withings)

**Co z nimi robić?**

**A) Pacjent widzi:**
- Dashboard zdrowia: Wykresy tygodniowe/miesięczne
- Trendy + alerty: "Puls spoczynkowy wzrósł 15% → sprawdź?"
- Korelacje: "Gdy śpisz <6h, poziom cukru rano wyższy" (dla diabetyków)

**B) Lekarz widzi (za zgodą):**
- Przed wizytą: "Pacjent X - puls śr. 95 bpm (za wysoki), sen 5h/noc"
- Podczas wizyty: "Wykres HRV z 30 dni"
- AI suggestions: "Wysoki stres + bóle głowy → nadciśnienie? Zalecić holter?"

**C) System reaguje:**

**Automated alerts:**
- SpO2 < 90% przez 10 min → "Wszystko OK? [Wezwać pomoc]"
- Puls >120 bpm w spoczynku → "Zmierz ciśnienie, zgłoś się do lekarza"

**Preventive care:**
- "Nie śpisz dobrze od 2 tygodni → teleporada psychiatra?" (mental health!)

**Research:**
- Anonimizowane dane do badań (za zgodą) - wartościowe dla pharma

**Privacy first:**
- ✅ Opt-in: Użytkownik wybiera co udostępnia
- ✅ Granular control: "Lekarz widzi tylko puls i sen, nie aktywność"
- ✅ GDPR compliance: Prawo do usunięcia danych

---

**🎯 PRIORYTETYZACJA IMPLEMENTACJI:**

**MVP (0-6 miesięcy):**
- ✅ AI Symptom Checker Poziom 1
- ✅ Marketplace z podstawowym rankingiem
- ✅ Podstawowe follow-up (SMS/email reminders)

**Phase 2 (6-12 miesięcy):**
- ✅ Wearables Tier 1 integration
- ✅ Personalizacja homepage
- ✅ AI asystent dla lekarza (opis wizyty)

**Phase 3 (rok+):**
- ✅ Advanced wearables + predictive health
- ✅ Dynamic pricing + marketplace gamification
- ✅ Pełny human + AI hybrid follow-up

**💎 KEY INSIGHT Branch 2:**
> **YourMedic to nie tylko "umów wizytę".**
> **To platforma, która łączy AI, wearables i telemedycynę w jeden inteligentny ekosystem,**
> **który dba o zdrowie pacjenta 24/7 - od objawów, przez wizytę, po follow-up i prewencję.**

---

## Idea Categorization

### Immediate Opportunities

_Ideas ready to implement now_

{{immediate_opportunities}}

### Future Innovations

_Ideas requiring development/research_

{{future_innovations}}

### Moonshots

_Ambitious, transformative concepts_

{{moonshots}}

### Insights and Learnings

_Key realizations from the session_

{{insights_learnings}}

## Action Planning

### Top 3 Priority Ideas

#### #1 Priority: {{priority_1_name}}

- Rationale: {{priority_1_rationale}}
- Next steps: {{priority_1_steps}}
- Resources needed: {{priority_1_resources}}
- Timeline: {{priority_1_timeline}}

#### #2 Priority: {{priority_2_name}}

- Rationale: {{priority_2_rationale}}
- Next steps: {{priority_2_steps}}
- Resources needed: {{priority_2_resources}}
- Timeline: {{priority_2_timeline}}

#### #3 Priority: {{priority_3_name}}

- Rationale: {{priority_3_rationale}}
- Next steps: {{priority_3_steps}}
- Resources needed: {{priority_3_resources}}
- Timeline: {{priority_3_timeline}}

## Reflection and Follow-up

### What Worked Well

{{what_worked}}

### Areas for Further Exploration

{{areas_exploration}}

### Recommended Follow-up Techniques

{{recommended_techniques}}

### Questions That Emerged

{{questions_emerged}}

### Next Session Planning

- **Suggested topics:** {{followup_topics}}
- **Recommended timeframe:** {{timeframe}}
- **Preparation needed:** {{preparation}}

---

_Session facilitated using the BMAD CIS brainstorming framework_
