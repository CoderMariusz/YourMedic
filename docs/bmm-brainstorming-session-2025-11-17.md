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

#### Branch 3: Podejścia Techniczne - Architektura i Implementacja

**🎯 Central Question:** JAK zbudować platformę skalowalna, bezpieczną i zgodną z regulacjami medycznymi dla 3 grup użytkowników?

---

**📱 FLUTTER CROSS-PLATFORM - Strategia Offline-First**

**A) Co MUSI działać offline - Podział według ról:**

**👤 PACJENT:**

✅ **MUSI działać offline:**
- Historia wizyt (ostatnie 6 miesięcy) - readonly
- Lista leków z przypomnieniami - readonly, notyfikacje działają
- Dokumenty PDF (zalecenia, wyniki) - cache lokalny
- Historia objawów w Symptom Checker - zapisz lokalnie, wyślij później
- Podstawowe dane profilu (imię, data urodzenia, alergie, grupa krwi)

❌ **NIE działa offline:**
- Umawianie nowych wizyt (live calendar)
- Płatności
- Czat/wideokonsultacja
- Wyszukiwanie lekarzy
- AI Symptom Checker (wymaga ML API)

**Storage strategy:**
- Hive dla structured data (wizyty, leki, profil)
- Cache lokalny PDF (max 100 MB)
- Background sync co 24h (WorkManager)

**👨‍⚕️ LEKARZ:**

✅ **MUSI działać offline (critical workflow):**
- Kalendarz wizyt DZIŚ + jutro (pełne dane pacjentów)
- Karty pacjentów z dzisiejszego dnia:
  - Podstawowe dane (ID, imię, kontakt)
  - Historia chorób (12 miesięcy)
  - Aktualne leki
  - **Alergie ⚠️ (ZAWSZE dostępne)**
  - Ostatnie 3 wizyty
- Tworzenie notatek offline:
  - SOAP notes zapisane lokalnie z flagą `pending_sync`
  - Upload przy powrocie internetu
  - Nie blokuje kolejnych wizyt
- Wystawianie recept DRAFT:
  - Draft lokalnie
  - Wysyłka do e-recepty gdy online

❌ **NIE działa offline:**
- Dodawanie NOWYCH pacjentów
- Pełna historia >12 miesięcy
- Powiadomienia SMS
- Wideokonsultacje
- Integracja EHR/lab

**Prefetch strategy:**
```dart
// Na początku dnia lub przy otwarciu app
Future<void> prefetchTodayData() async {
  if (await hasConnection()) {
    // Pobierz wizyty dziś + jutro
    final appointments = await api.getAppointments(
      from: DateTime.now(),
      to: DateTime.now().add(Duration(days: 1))
    );

    // Dla każdej wizyty - dane pacjenta
    for (var apt in appointments) {
      final patientData = await api.getPatientEssentials(apt.patientId);
      await hive.savePatientCache(patientData);
    }
  }
}

// Po wizycie - queue do sync
Future<void> saveVisitNote(VisitNote note) async {
  await hive.saveVisitNote(note, synced: false);

  if (await hasConnection()) {
    await _syncPendingNotes();
  }
}
```

**Cache management:**
- Max 500 MB (30 dni wizyt + dokumenty)
- Auto-clean >60 dni
- Priorytet: dzisiejsze > historia > dokumenty

**🏥 KLINIKA/ADMIN:**
- ✅ Offline: Podstawowy dashboard (cached stats), lista personelu
- ❌ Online-first: Real-time stats, edycja grafików, zarządzanie dostępami

---

**B) Synchronizacja Konfliktów - Konkretne Scenariusze:**

**Scenariusz 1: Pacjent edytuje dane offline + online jednocześnie**

**Problem:**
- Komórka offline: zmiana adresu na "Nowa 10"
- Żona online: zmiana na "Stara 5"
- Konflikt przy sync

**Rozwiązanie: Last-Write-Wins + timestamp**
```dart
// Backend endpoint
PUT /api/patient/profile
{
  "address": "Nowa 10",
  "lastModified": "2025-11-17T10:30:00Z"
}

// Backend check:
if (request.lastModified < dbRecord.lastModified) {
  return {
    status: "conflict",
    serverVersion: dbRecord,
    yourVersion: request
  };
}

// Flutter handling:
try {
  await api.updateProfile(localProfile);
} on ConflictException catch (e) {
  showDialog(
    title: "Konflikt danych",
    content: "Dane zmienione na innym urządzeniu. Która wersja poprawna?",
    actions: [
      "Zachowaj moją (${e.yourVersion.address})",
      "Użyj nowszej (${e.serverVersion.address})"
    ]
  );
}
```

**Strategy:**
- Większość pól: Last-Write-Wins auto (adres, telefon)
- Krytyczne pola: Manual resolve (alergie, grupa krwi)

**Scenariusz 2: Lekarz offline zapisuje, pacjent online odwołał**

**Problem:**
- Lekarz offline prowadzi wizytę, zapisuje notatkę
- Pacjent online odwołał 5 min wcześniej
- Co z notatką przy sync?

**Rozwiązanie: Server reconciliation**
```python
# Backend check
if appointment.status == "cancelled":
  # NIE odrzucaj notatki!
  appointment.status = "visit_happened_despite_cancellation"
  send_alert_to_admin()
  return {
    "warning": "Pacjent odwołał, ale wizyta się odbyła",
    "action_required": true
  }
```

**Best practice:**
- Prefetch rano → lekarz wie kto odwołał
- Przycisk "Restore appointment" przed zapisem notatki

**Scenariusz 3: Field-level merge dla notatek**

```javascript
// Backend merge strategy
function mergeVisitNotes(serverNote, clientNote) {
  return {
    // Tekst: append jeśli różne
    diagnosis: mergeSections(serverNote.diagnosis, clientNote.diagnosis),

    // Leki: union (bez duplikatów)
    medications: union(serverNote.medications, clientNote.medications),

    // Metadane: last-write-wins
    lastModifiedAt: max(server.lastModifiedAt, client.lastModifiedAt)
  };
}

function mergeSections(server, client) {
  if (server === client) return server;
  if (!server) return client;
  if (!client) return server;

  // Oba różne → append
  return `${server}\n\n[DODANE OFFLINE]:\n${client}`;
}
```

**Scenariusz 4: Race condition - rezerwacja slotu**

**Problem:** Dwóch pacjentów klika ten sam slot jednocześnie

**Rozwiązanie: Optimistic locking**
```sql
-- Postgres transaction
BEGIN;

SELECT * FROM appointments
WHERE doctor_id = 'doc_123'
  AND slot_time = '2025-11-18 10:00:00'
  AND status = 'available'
FOR UPDATE NOWAIT; -- Pierwszy dostaje lock

UPDATE appointments
SET status = 'booked', patient_id = 'pat_456'
WHERE id = 'apt_789';

COMMIT;
-- Drugi dostaje error "slot taken"
```

```dart
// Flutter handling
try {
  await api.bookAppointment(slot);
  showSuccess("Wizyta zarezerwowana!");
} on SlotTakenException {
  showError("Termin zajęty przez inną osobę. Wybierz inny.");
  await refreshCalendar();
}
```

**C) Conflict Resolution Priority Matrix:**

| Typ danych | Strategia | Dlaczego |
|-----------|-----------|----------|
| Dane osobowe | Last-write-wins + timestamp | Rzadko jednocześnie |
| Alergie/Grupa krwi | Manual resolve | Krytyczne dla bezpieczeństwa |
| Notatki lekarza | Field-level merge | Obie wersje ważne |
| Status wizyty | Server wins | Single source of truth |
| Przypomnienia | Client wins | Lokalne preferencje |
| Kalendarz | Optimistic locking | Pierwszy = jego |

---

**🏥 MEDICAL DEVICE CERTIFICATION - EU MDR Compliance**

**A) Czy Flutter app musi być certyfikowana?**

**Odpowiedź: ZALEŻY od funkcjonalności** 🎯

**Jest Medical Device jeśli:**
- ✅ Diagnozuje choroby (nawet "wspomagająco")
- ✅ Zapobiega chorobom (algorytm predykcyjny)
- ✅ Monitoruje parametry życiowe + rekomendacje kliniczne
- ✅ Wspiera decyzje terapeutyczne

**NIE jest Medical Device jeśli:**
- ❌ Tylko booking system
- ❌ Tylko przechowuje dane (EHR bez analizy)
- ❌ Edukuje ogólnie (nie personalizowane)
- ❌ Komunikacja pacjent↔lekarz (czat, video)

**B) YourMedic - Analiza komponent:**

| Feature | Medical Device? | Klasa | Wymaga CE? |
|---------|----------------|-------|------------|
| Booking wizyt | ❌ NIE | - | NIE |
| Czat/Video | ❌ NIE | - | NIE |
| Historia (readonly) | ❌ NIE | - | NIE |
| Przypomnienia o lekach | ⚠️ Szara strefa | I | TAK* |
| **AI Symptom Checker** | ✅ **TAK** | **IIa** | **TAK** |
| **AI asystent lekarza** | ✅ **TAK** | **IIa** | **TAK** |
| **Wearables monitoring** | ✅ **TAK** | **IIa/IIb** | **TAK** |
| Marketplace | ❌ NIE | - | NIE |

*Przypomnienia: Prosty alarm "weź lek o 18:00" = NIE device | "Nie brałeś 2 dni → kontakt z lekarzem" = TAK device

**C) Strategia: MODULAR CERTIFICATION** 🎯

**Architektura:**
```
YourMedic App (Flutter)
│
├── Core App (NIE medical device)
│   ├── Authentication
│   ├── Booking system
│   ├── Payments
│   ├── Chat/Video
│   ├── Calendar
│   └── Profile management
│
└── Medical Modules (Certyfikowane osobno)
    ├── AI Symptom Checker (Class IIa) ← CE Mark
    ├── AI Doctor Assistant (Class IIa) ← CE Mark
    └── Wearables Monitor (Class IIb) ← CE Mark
```

**Implementation:**
```dart
// Core app - NIE wymaga certyfikacji
class YourMedicApp {
  BookingService booking;
  ChatService chat;
  PaymentService payments;

  // Opcjonalne moduły (dynamicznie ładowane)
  MedicalModule? symptomChecker;
  MedicalModule? aiAssistant;
}

// Certyfikowany moduł
@MedicalDevice(
  classification: "IIa",
  certNumber: "CE12345"
)
class SymptomCheckerModule extends MedicalModule {
  // Ten kod podlega audytowi Notified Body
  Future<SymptomAnalysis> analyze(List<Symptom> symptoms) {
    // Wywołanie do certyfikowanego ML API
  }
}
```

**Zalety:**
- ✅ Core app: Swobodny deployment (OTA updates, iteracje)
- ✅ Medical modules: Kontrolowany proces certyfikacyjny
- ✅ Geographic flexibility: Różne kraje = różne moduły
- ✅ Cost optimization: Certyf tylko to co trzeba

**D) Proces Certyfikacji Class IIa:**

**1. Dokumentacja techniczna (6-12 miesięcy):**
- Software development lifecycle (IEC 62304)
- Risk management file (ISO 14971)
- Clinical evaluation report
- Usability engineering (IEC 62366)
- Cybersecurity docs (MDR Annex I)

**2. Notified Body assessment:**
- Wybór: BSI, TÜV SÜD, etc.
- Audyt dokumentacji + code review
- **Koszt: €20,000 - €50,000** dla Class IIa
- **Czas: 3-6 miesięcy**

**3. CE Mark:**
- Ważność: 5 lat → re-certification
- Surveillance: coroczne audyty
- Post-market: adverse events tracking

**4. Software updates:**
- ⚠️ Minor bug fix → nie wymaga nowego CE
- ⚠️ New feature/algorithm → TAK, wymaga review Notified Body

**E) Deployment Strategy - Hybrid Approach (BEST PRACTICE):**

**ML model na backendzie (nie w app):**

```dart
// Flutter app (NIE certyfikowane)
class SymptomCheckerUI {
  Future<SymptomAnalysis> checkSymptoms(List<Symptom> symptoms) {
    // Wysyła do API
    return http.post('/api/v2/symptom-check', body: symptoms);
  }
}
```

```python
# Backend Python (CERTYFIKOWANY jako SaMD)
@medical_device_endpoint
@app.route('/api/v2/symptom-check', methods=['POST'])
def symptom_check():
    symptoms = request.json
    # Ten kod jest certyfikowany
    result = ml_model.predict(symptoms)
    return jsonify(result)
```

**✅ Zalety:**
- Flutter app: Swobodny deployment
- Backend API: Kontrolowane zmiany
- API versioning (v1, v2, v3): Łatwe migracje
- Rollback: Zmiana endpoint w config
- Compliance: Backend = "standalone software", Frontend = "accessory" (łagodniejsze wymogi)

**F) Cost Estimate dla Certyfikacji:**
- Notified Body: €30,000
- Regulatory consultant: €15,000
- Clinical evaluation study: €10,000
- **TOTAL: ~€55,000** dla Class IIa

**G) Strategia dla YourMedic - 3 fazy:**

**Phase 1 (MVP 0-6m): AVOID medical device classification**
- Launch Core App (booking, chat, marketplace)
- Symptom Checker jako "educational tool":
  - "Not medical advice"
  - "For informational purposes only"
  - Zero personalized recommendations

**Phase 2 (6-12m): Prepare for certification**
- Zbieraj dane użytkowników (clinical evaluation)
- Buduj dokumentację techniczną
- Hire regulatory consultant (€5-10k)
- Design modular architecture

**Phase 3 (12m+): Certify AI modules**
- Submit do Notified Body
- Podczas review: Core App updates normalnie
- Po certyfikacji: Medical features jako opt-in

**H) Risk Mitigation - Alternatywy:**

**Opcja 1: Partnership model**
- YourMedic = platforma (non-device)
- Lekarz używa SWOJEGO certyfikowanego software
- Ty = "infrastructure provider"

**Opcja 2: Geographic segmentation**
- EU/UK: No medical features (tylko booking)
- US: FDA "low-risk" exemption
- India/LatAm: Mniej restrykcyjne

**Opcja 3: B2B pivot**
- Sprzedaj klinikom jako "practice management"
- Klinika = compliance owner
- Ty = narzędzia dostarczasz

**💎 KEY INSIGHTS Branch 3 (Część 1):**
> **Offline-first:** Pacjent cache 6m + 100MB, Lekarz prefetch dziś+jutro 500MB, Last-write-wins + timestamp dla konfliktów
> **Medical Device:** Core app NIE device (swobodny deploy), AI modules certyfikowane osobno (Class IIa), Backend ML strategy (€55k, 9-12 miesięcy)
> **MVP Strategy:** Launch bez medical features, certyfikuj później, modular architecture od początku

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
