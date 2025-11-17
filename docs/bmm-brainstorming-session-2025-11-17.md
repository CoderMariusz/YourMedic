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

**━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━**

### **Branch 3 (Part 2): Backend Architecture + Integracje**

**User Constraints & Decisions:**
- ✅ AI/ML w oddzielnym serwisie (separate ML microservice)
- ✅ Brak existing team - otwarty na sugestie technologiczne
- ✅ Priorytet: Speed to market w MVP, ale long-term scalability później

---

#### **A) Backend Framework Recommendation: Hybrid Approach**

**Propozycja: NestJS (main API) + Python ML Service**

**Rationale:**

**NestJS dla Core API:**
```
✅ Speed to market (MVP priorytet #1)
   - TypeScript = Flutter dev również może backend wspierać
   - Built-in: Auth, WebSocket, GraphQL, validation
   - Modular architecture out of the box
   - Swagger auto-generation dla docs

✅ Long-term scalability
   - Microservices-ready (już projekt pod to)
   - Dependency injection = testable code
   - Large ecosystem (Prisma, TypeORM, Bull queues)
   - Enterprise adoption (Adidas, Roche, Trivia Crack)

✅ Real-time features
   - WebSocket dla live chat (Lekarz ↔ Pacjent)
   - Server-sent events dla notyfikacji
   - Native support, zero third-party libs

✅ Polish talent pool
   - TypeScript = najpopularniejszy w PL (większy niż Python backend devs)
   - Junior-friendly = niższe koszty hiring
```

**Python dla ML Service:**
```
✅ ML Ecosystem
   - TensorFlow, PyTorch, scikit-learn
   - Hugging Face transformers dla NLP (symptom parsing)
   - FastAPI = production-ready ML serving

✅ Separation of concerns
   - ML service skaluje niezależnie
   - Core API może być w maintenance mode podczas ML updates
   - Certyfikacja Medical Device = tylko ML service

✅ Cost efficiency
   - ML service: GPU instances (AWS p3, Google TPU)
   - Core API: Standard compute (cheaper)
   - Separate scaling = $$$ savings
```

**Architecture Diagram:**

```
┌─────────────────────────────────────────────────────────┐
│                    Flutter App                           │
│          (iOS, Android, Web - Offline-first)            │
└─────────────────┬───────────────────────────────────────┘
                  │
                  ▼
        ┌─────────────────────┐
        │   API Gateway       │
        │   (AWS API GW /     │
        │    Kong / nginx)    │
        └──────────┬──────────┘
                   │
        ┌──────────┴──────────────────────┐
        │                                  │
        ▼                                  ▼
┌──────────────────┐            ┌──────────────────────┐
│   NestJS API     │            │  Python ML Service   │
│   (Core Backend) │◄───────────┤  (FastAPI)           │
│                  │  gRPC/REST │                      │
│  - Auth          │            │  - Symptom Checker   │
│  - Appointments  │            │  - Risk prediction   │
│  - Marketplace   │            │  - Photo analysis    │
│  - Chat          │            │  - Wearables ML      │
│  - Notifications │            │                      │
│  - FHIR adapter  │            │  ** Class IIa **     │
└────────┬─────────┘            └──────────────────────┘
         │
         ▼
┌──────────────────┐
│   PostgreSQL     │
│   (Primary DB)   │
│                  │
│  + Redis Cache   │
│  + S3 (files)    │
└──────────────────┘
```

**Code Example - NestJS Core API:**

```typescript
// appointments.controller.ts
@Controller('appointments')
@UseGuards(JwtAuthGuard)
export class AppointmentsController {
  constructor(
    private appointmentsService: AppointmentsService,
    private mlServiceClient: MlServiceClient, // gRPC client
  ) {}

  @Post()
  async createAppointment(
    @Body() dto: CreateAppointmentDto,
    @CurrentUser() user: User,
  ) {
    // 1. Validate slot availability
    const slot = await this.appointmentsService.findSlot(dto.slotId);
    if (!slot.available) throw new ConflictException('Slot taken');

    // 2. Create appointment (optimistic locking)
    const appointment = await this.appointmentsService.create({
      ...dto,
      patientId: user.id,
      version: 1, // dla conflict resolution
    });

    // 3. Call ML service dla risk score (async)
    this.mlServiceClient
      .calculateRiskScore({
        patientId: user.id,
        symptoms: dto.symptoms,
      })
      .subscribe((risk) => {
        // Update appointment z risk score
        this.appointmentsService.updateRiskScore(appointment.id, risk.score);
      });

    return appointment;
  }

  @Get()
  async getUserAppointments(@CurrentUser() user: User) {
    return this.appointmentsService.findByUser(user.id, {
      include: { doctor: true, clinic: true },
    });
  }
}
```

**Code Example - Python ML Service:**

```python
# ml_service/main.py
from fastapi import FastAPI, HTTPException
from pydantic import BaseModel
import tensorflow as tf

app = FastAPI()

# Load certified model (immutable version)
model = tf.keras.models.load_model('/models/symptom_checker_v2.1_certified.h5')

class SymptomRequest(BaseModel):
    patient_id: str
    symptoms: list[str]
    age: int
    sex: str
    medical_history: list[str] = []

@app.post("/api/v1/symptom-check")
async def check_symptoms(req: SymptomRequest):
    """
    Class IIa Medical Device Software
    Certified: 2025-03-15 | Notified Body: TÜV SÜD
    Version: 2.1 (DO NOT MODIFY without recertification)
    """

    # Preprocessing
    features = preprocess_symptoms(
        symptoms=req.symptoms,
        age=req.age,
        sex=req.sex,
        history=req.medical_history
    )

    # Prediction
    prediction = model.predict(features)

    # Post-processing (certified logic)
    result = {
        "possible_conditions": extract_top_n(prediction, n=3),
        "urgency_level": calculate_urgency(prediction),
        "recommended_action": get_recommendation(prediction),
        "disclaimer": "This is not a diagnosis. Consult a healthcare professional.",
        "model_version": "2.1",
        "certified": True
    }

    # Red flags check (auto-escalate)
    if has_red_flags(req.symptoms):
        result["urgency_level"] = "EMERGENCY"
        result["recommended_action"] = "Seek immediate emergency care"

    return result
```

---

#### **B) Multi-Tenancy Architecture dla Klinik**

**Problem:** 1000+ klinik, każda z własnym:
- Zespołem lekarzy
- Grafik scheduling rules
- Branding (logo, colors)
- Cennik (marketplace pricing)

**Solution: Schema-based Multi-tenancy (PostgreSQL)**

**Dlaczego schema-based, nie database-per-tenant?**
```
✅ Cost: 1 database vs 1000 databases
✅ Backups: 1 backup job vs 1000
✅ Migrations: Apply once vs 1000x
✅ Cross-tenant analytics (aggregated stats)
✅ Shared resources (doctors working w >1 clinic)

❌ Teoretycznie słabsza izolacja (ale wystarczająca dla GDPR/HIPAA)
```

**Implementation:**

```typescript
// tenant.middleware.ts
@Injectable()
export class TenantMiddleware implements NestMiddleware {
  use(req: Request, res: Response, next: NextFunction) {
    // Extract tenant from subdomain lub custom header
    const tenantId = this.extractTenantId(req);

    if (!tenantId) {
      throw new UnauthorizedException('No tenant context');
    }

    // Set PostgreSQL schema for this request
    req['tenantId'] = tenantId;
    next();
  }

  private extractTenantId(req: Request): string | null {
    // Option 1: Subdomain (luxmed.yourmedic.pl)
    const subdomain = req.hostname.split('.')[0];
    if (subdomain !== 'www' && subdomain !== 'api') {
      return subdomain;
    }

    // Option 2: Custom header (mobile apps)
    return req.headers['x-tenant-id'] as string;
  }
}

// tenant.interceptor.ts (auto-inject tenant w queries)
@Injectable()
export class TenantInterceptor implements NestInterceptor {
  intercept(context: ExecutionContext, next: CallHandler): Observable<any> {
    const request = context.switchToHttp().getRequest();
    const tenantId = request['tenantId'];

    // Set PostgreSQL search_path dla tego połączenia
    return from(
      this.prisma.$executeRaw`SET search_path TO tenant_${tenantId}, public`
    ).pipe(
      switchMap(() => next.handle())
    );
  }
}
```

**Database Schema:**

```sql
-- Shared public schema (cross-tenant data)
CREATE TABLE public.tenants (
  id UUID PRIMARY KEY,
  name VARCHAR(255),
  subdomain VARCHAR(100) UNIQUE,
  plan VARCHAR(50), -- 'free', 'pro', 'enterprise'
  created_at TIMESTAMP DEFAULT NOW()
);

-- Per-tenant schema (isolated data)
CREATE SCHEMA tenant_luxmed;

CREATE TABLE tenant_luxmed.doctors (
  id UUID PRIMARY KEY,
  user_id UUID REFERENCES public.users(id), -- Doctor może być w >1 tenant
  specialization VARCHAR(100),
  bio TEXT,
  hourly_rate DECIMAL(10, 2)
);

CREATE TABLE tenant_luxmed.appointments (
  id UUID PRIMARY KEY,
  patient_id UUID REFERENCES public.users(id),
  doctor_id UUID REFERENCES tenant_luxmed.doctors(id),
  slot_start TIMESTAMP,
  slot_end TIMESTAMP,
  status VARCHAR(50),
  -- RLS (Row Level Security) for extra paranoia
  CONSTRAINT tenant_isolation CHECK (tenant_id = current_setting('app.current_tenant')::UUID)
);
```

**Row-Level Security (dodatkowa warstwa):**

```sql
-- Enable RLS
ALTER TABLE tenant_luxmed.appointments ENABLE ROW LEVEL SECURITY;

-- Policy: User może czytać tylko swoje appointments
CREATE POLICY appointments_isolation ON tenant_luxmed.appointments
  FOR ALL
  USING (
    patient_id = current_setting('app.current_user')::UUID
    OR
    doctor_id IN (
      SELECT id FROM tenant_luxmed.doctors
      WHERE user_id = current_setting('app.current_user')::UUID
    )
  );
```

---

#### **C) FHIR/HL7 Integration Strategy**

**Problem:** Kliniki mają existing EHR systems (eKARTA, Kamsoft, Mediporta w PL)
**Musisz:** Import patient history, export consultation notes

**FHIR (Fast Healthcare Interoperability Resources):**
```
✅ Modern standard (2011+, aktywny development)
✅ RESTful API = easy integration
✅ JSON format = developer-friendly
✅ Resources: Patient, Appointment, MedicationRequest, Observation
✅ EU requirement dla health data exchange (od 2025)
```

**HL7 v2 (Legacy):**
```
❌ Pipe-delimited messages (ADT^A01|...|...)
❌ Complex parsing
✅ Still 80% of hospital systems w PL
✅ Real-time feeds (patient admission, lab results)
```

**Hybrid Strategy:**

**Phase 1 (MVP 0-6m): FHIR only (modern kliniki)**
```typescript
// fhir.service.ts
import { Client } from 'fhir-kit-client';

@Injectable()
export class FhirService {
  private client: Client;

  constructor() {
    this.client = new Client({
      baseUrl: 'https://clinic-ehr.example.com/fhir',
      customHeaders: {
        Authorization: `Bearer ${process.env.EHR_API_KEY}`,
      },
    });
  }

  async importPatientHistory(patientId: string) {
    // Fetch FHIR Patient resource
    const patient = await this.client.read({
      resourceType: 'Patient',
      id: patientId,
    });

    // Fetch Observations (lab results, vitals)
    const observations = await this.client.search({
      resourceType: 'Observation',
      searchParams: {
        patient: patientId,
        category: 'vital-signs',
        _sort: '-date',
        _count: 100,
      },
    });

    // Transform FHIR → YourMedic schema
    return {
      demographics: this.mapPatientDemographics(patient),
      vitals: observations.entry.map(obs => this.mapObservation(obs.resource)),
    };
  }

  async exportConsultationNote(appointmentId: string) {
    const appointment = await this.appointmentsService.findOne(appointmentId);

    // Create FHIR Encounter resource
    const encounter = {
      resourceType: 'Encounter',
      status: 'finished',
      class: { code: 'AMB' }, // Ambulatory
      subject: { reference: `Patient/${appointment.patientId}` },
      participant: [{
        individual: { reference: `Practitioner/${appointment.doctorId}` }
      }],
      period: {
        start: appointment.startTime,
        end: appointment.endTime,
      },
    };

    // POST to clinic EHR
    return this.client.create({
      resourceType: 'Encounter',
      body: encounter,
    });
  }
}
```

**Phase 2 (6-12m): HL7 adapter dla legacy systems**
```typescript
// hl7.service.ts
import hl7 from 'simple-hl7';

@Injectable()
export class Hl7Service {
  async parseAdtMessage(hl7Message: string) {
    const msg = new hl7.Message(hl7Message);

    // ADT^A01 = Patient admission
    if (msg.get('MSH.9').toString() === 'ADT^A01') {
      return {
        patientId: msg.get('PID.3').toString(), // Patient ID
        name: {
          family: msg.get('PID.5.1').toString(),
          given: msg.get('PID.5.2').toString(),
        },
        birthDate: this.parseHL7Date(msg.get('PID.7').toString()),
        gender: msg.get('PID.8').toString(),
      };
    }
  }

  async sendORMMessage(appointment: Appointment) {
    // ORM^O01 = Order message (consultation request)
    const msg = new hl7.Message({
      messageHeader: {
        msh_9_1: 'ORM',
        msh_9_2: 'O01',
        msh_10: this.generateMessageId(),
      },
      patient: {
        pid_3: appointment.patientId,
      },
      order: {
        orc_1: 'NW', // New order
        orc_5: 'A', // Active
      },
    });

    // Send via MLLP (Minimal Lower Layer Protocol)
    return this.mllpClient.send(msg.toString());
  }
}
```

**Recommendation dla MVP:**
```
Phase 1: Manual CSV import/export (Excel templates)
  ↓
Phase 2: FHIR API dla 20% modern kliniki
  ↓
Phase 3: HL7 adapter dla 80% legacy systems
```

---

#### **D) Security & Encryption (GDPR + HIPAA Compliance)**

**Threat Model:**

```
1. Data at rest (database breach)
   → Solution: Transparent Data Encryption (TDE)

2. Data in transit (man-in-the-middle)
   → Solution: TLS 1.3, certificate pinning

3. Application-level access (insider threat)
   → Solution: Field-level encryption + audit logs

4. Backup leaks
   → Solution: Encrypted backups, key rotation
```

**Implementation:**

**A) Transparent Data Encryption (PostgreSQL):**
```bash
# Enable pgcrypto extension
CREATE EXTENSION pgcrypto;

# Encrypt sensitive columns
CREATE TABLE patients (
  id UUID PRIMARY KEY,
  email VARCHAR(255),
  -- PESEL (Polish national ID) - must be encrypted
  pesel_encrypted BYTEA,
  -- Medical history - sensitive
  medical_history_encrypted BYTEA
);

# Insert with encryption
INSERT INTO patients (id, email, pesel_encrypted, medical_history_encrypted)
VALUES (
  gen_random_uuid(),
  'jan.kowalski@example.com',
  pgp_sym_encrypt('92010112345', current_setting('app.encryption_key')),
  pgp_sym_encrypt('{"conditions": ["diabetes"]}', current_setting('app.encryption_key'))
);

# Read with decryption
SELECT
  id,
  email,
  pgp_sym_decrypt(pesel_encrypted, current_setting('app.encryption_key')) AS pesel,
  pgp_sym_decrypt(medical_history_encrypted, current_setting('app.encryption_key')) AS medical_history
FROM patients;
```

**B) Application-Level Encryption (NestJS):**
```typescript
// encryption.service.ts
import * as crypto from 'crypto';

@Injectable()
export class EncryptionService {
  private algorithm = 'aes-256-gcm';
  private key: Buffer;

  constructor(private configService: ConfigService) {
    // Key from AWS KMS lub HashiCorp Vault
    this.key = Buffer.from(
      this.configService.get('ENCRYPTION_KEY'),
      'hex'
    );
  }

  encrypt(text: string): { encrypted: string; iv: string; tag: string } {
    const iv = crypto.randomBytes(16);
    const cipher = crypto.createCipheriv(this.algorithm, this.key, iv);

    let encrypted = cipher.update(text, 'utf8', 'hex');
    encrypted += cipher.final('hex');

    const tag = cipher.getAuthTag();

    return {
      encrypted,
      iv: iv.toString('hex'),
      tag: tag.toString('hex'),
    };
  }

  decrypt(encrypted: string, iv: string, tag: string): string {
    const decipher = crypto.createDecipheriv(
      this.algorithm,
      this.key,
      Buffer.from(iv, 'hex')
    );

    decipher.setAuthTag(Buffer.from(tag, 'hex'));

    let decrypted = decipher.update(encrypted, 'hex', 'utf8');
    decrypted += decipher.final('utf8');

    return decrypted;
  }
}

// patient.entity.ts
@Entity()
export class Patient {
  @PrimaryGeneratedColumn('uuid')
  id: string;

  @Column()
  email: string;

  @Column({ type: 'text' })
  peselEncrypted: string;

  @Column({ type: 'text' })
  peselIv: string;

  @Column({ type: 'text' })
  peselTag: string;

  // Virtual field (nie zapisywane w DB)
  pesel?: string;

  // Encrypt before save
  @BeforeInsert()
  @BeforeUpdate()
  encryptSensitiveData() {
    if (this.pesel) {
      const encrypted = this.encryptionService.encrypt(this.pesel);
      this.peselEncrypted = encrypted.encrypted;
      this.peselIv = encrypted.iv;
      this.peselTag = encrypted.tag;
      delete this.pesel; // Remove plaintext
    }
  }

  // Decrypt after load
  @AfterLoad()
  decryptSensitiveData() {
    if (this.peselEncrypted) {
      this.pesel = this.encryptionService.decrypt(
        this.peselEncrypted,
        this.peselIv,
        this.peselTag
      );
    }
  }
}
```

**C) Audit Logging (GDPR Art. 30 requirement):**
```typescript
// audit.interceptor.ts
@Injectable()
export class AuditInterceptor implements NestInterceptor {
  constructor(private auditService: AuditService) {}

  intercept(context: ExecutionContext, next: CallHandler): Observable<any> {
    const req = context.switchToHttp().getRequest();
    const user = req.user;

    const auditLog = {
      userId: user?.id,
      action: `${req.method} ${req.url}`,
      ip: req.ip,
      userAgent: req.headers['user-agent'],
      timestamp: new Date(),
      resourceType: this.extractResourceType(req.url),
      resourceId: req.params.id,
    };

    // Log to separate audit database (immutable, append-only)
    this.auditService.log(auditLog);

    return next.handle();
  }
}

// audit.entity.ts
@Entity('audit_logs')
export class AuditLog {
  @PrimaryGeneratedColumn('uuid')
  id: string;

  @Column()
  userId: string;

  @Column()
  action: string; // "GET /patients/123"

  @Column()
  ip: string;

  @Column({ type: 'timestamp', default: () => 'CURRENT_TIMESTAMP' })
  timestamp: Date;

  @Column()
  resourceType: string; // "Patient", "Appointment"

  @Column({ nullable: true })
  resourceId: string;

  // IMMUTABLE - no updates/deletes allowed
  @BeforeUpdate()
  preventUpdates() {
    throw new Error('Audit logs are immutable');
  }
}
```

**D) Certificate Pinning (Flutter → Backend):**
```dart
// lib/services/http_client.dart
import 'package:dio/dio.dart';
import 'package:dio/io.dart';

class SecureHttpClient {
  static Dio createSecureClient() {
    final dio = Dio();

    // Certificate pinning - tylko YOUR server certificates
    (dio.httpClientAdapter as IOHttpClientAdapter).onHttpClientCreate =
      (client) {
        client.badCertificateCallback = (cert, host, port) {
          // SHA-256 fingerprint of YOUR prod certificate
          const expectedFingerprint =
            'AA:BB:CC:DD:EE:FF:00:11:22:33:44:55:66:77:88:99:AA:BB:CC:DD:EE:FF:00:11:22:33:44:55:66:77:88:99';

          final certFingerprint = cert.sha256.map((byte) =>
            byte.toRadixString(16).padLeft(2, '0')).join(':').toUpperCase();

          return certFingerprint == expectedFingerprint;
        };
        return client;
      };

    return dio;
  }
}
```

**E) Key Management Strategy:**

```
Development: .env file (rotating every 90 days)
  ↓
Staging: AWS Secrets Manager (auto-rotation)
  ↓
Production: AWS KMS + HashiCorp Vault
  - Master key w KMS (hardware security module)
  - Data encryption keys w Vault (dynamic secrets)
  - Auto-rotation every 30 days
  - Audit trail dla każdego key access
```

---

**💎 KEY INSIGHTS Branch 3 (Część 2):**
> **Backend:** NestJS (Core API, TypeScript, speed to market) + Python FastAPI (ML service, separate certyfikacja, GPU scaling)
> **Multi-tenancy:** Schema-based PostgreSQL (tenant_luxmed, tenant_medicover), Row-Level Security, subdomain routing
> **FHIR/HL7:** MVP = manual CSV, Phase 2 = FHIR dla modern kliniki, Phase 3 = HL7 adapter dla legacy (80% PL market)
> **Security:** TDE + field-level encryption (AES-256-GCM), audit logs (immutable), certificate pinning, AWS KMS key management

**━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━**

### **Branch 4: Technical Risks & Mitigation Strategies**

**Category Analysis:** Offline-first, Medical certification, Security, Scale, Integration

---

#### **RISK #1: Offline Sync Conflicts - Data Corruption**

**Severity:** 🔴 CRITICAL
**Probability:** Medium (20-30% users będą offline >1h dziennie)
**Impact:** Data loss = lawsuit + patient harm

**Scenario:**
```
1. Lekarz offline edits patient record v1 → v2_local
2. Inny lekarz w clinic edits v1 → v2_server (online)
3. Pierwszy lekarz sync → v2_local overwrites v2_server (last-write-wins)
4. RESULT: Drugi lekarz changes = LOST
```

**Mitigation Strategies:**

**A) Implement CRDT (Conflict-Free Replicated Data Types):**
```dart
// lib/models/patient_record_crdt.dart
import 'package:crdt/crdt.dart';

class PatientRecordCRDT {
  final Crdt crdt;

  PatientRecordCRDT() : crdt = Crdt.hlc();

  // Merge offline changes without conflicts
  void updateMedicalHistory(String entry, DateTime timestamp) {
    crdt.put('medical_history_${timestamp.millisecondsSinceEpoch}', entry);
  }

  // Automatic merge during sync
  void merge(Map<String, dynamic> remoteChangeset) {
    crdt.merge(remoteChangeset);
    // All changes preserved, chronologically ordered
  }

  List<String> getMedicalHistory() {
    return crdt
      .getMap()
      .entries
      .where((e) => e.key.startsWith('medical_history_'))
      .map((e) => e.value as String)
      .toList();
  }
}
```

**B) Operational Transform dla Real-time Collaborative Editing:**
```typescript
// backend: collaborative-notes.service.ts
import * as ot from 'ot';

@Injectable()
export class CollaborativeNotesService {
  // Track document versions
  private documentVersions = new Map<string, number>();

  async applyOperation(
    documentId: string,
    operation: ot.Operation,
    baseVersion: number
  ) {
    const currentVersion = this.documentVersions.get(documentId) || 0;

    if (baseVersion < currentVersion) {
      // Transform operation against all intermediate changes
      const transformedOp = this.transformAgainstHistory(
        documentId,
        operation,
        baseVersion,
        currentVersion
      );
      return transformedOp;
    }

    // Apply and increment version
    await this.applyToDatabase(documentId, operation);
    this.documentVersions.set(documentId, currentVersion + 1);
  }
}
```

**C) Conflict Detection UI:**
```dart
// Show user conflicts instead of silent override
class ConflictResolutionScreen extends StatelessWidget {
  final Conflict conflict;

  @override
  Widget build(BuildContext context) {
    return AlertDialog(
      title: Text('Konflikt danych wykryty'),
      content: Column(
        children: [
          Text('Twoja wersja (offline):'),
          Text(conflict.localVersion, style: TextStyle(color: Colors.blue)),
          SizedBox(height: 16),
          Text('Wersja z serwera:'),
          Text(conflict.serverVersion, style: TextStyle(color: Colors.green)),
        ],
      ),
      actions: [
        TextButton(
          onPressed: () => resolveConflict(ConflictStrategy.KEEP_LOCAL),
          child: Text('Użyj mojej wersji'),
        ),
        TextButton(
          onPressed: () => resolveConflict(ConflictStrategy.KEEP_SERVER),
          child: Text('Użyj wersji z serwera'),
        ),
        TextButton(
          onPressed: () => resolveConflict(ConflictStrategy.MERGE),
          child: Text('Scal obie (CRDT)'),
        ),
      ],
    );
  }
}
```

**Cost:** ~80h dev time + 3rd party CRDT library (~$0, open-source)
**Timeline:** Implement before beta launch
**Fallback:** Manual conflict resolution UI (always ask user)

---

#### **RISK #2: Medical Device Certification Delays**

**Severity:** 🟠 HIGH
**Probability:** High (70% certifications take longer than planned)
**Impact:** 9-12 months delay = burn rate crisis

**Scenario:**
```
1. Submit AI Symptom Checker for Class IIa cert (Month 12)
2. Notified Body finds gap in clinical evaluation data
3. Must conduct additional study (6 months + €20k)
4. Resubmit Month 18
5. Approval Month 24
6. RESULT: 12-month delay, 2x budget overrun
```

**Mitigation Strategies:**

**A) Pre-submission Consultation:**
```
Month 6: Hire regulatory consultant (€10k)
  ↓ Gap analysis of current AI module
Month 8: Pre-submission meeting z Notified Body (TÜV SÜD)
  ↓ Get feedback BEFORE official submission
Month 10: Address gaps (clinical data, risk management)
  ↓
Month 12: Official submission (higher chance of success)
```

**B) Phased Feature Release:**
```
Phase 1 (MVP): NO medical device features
  - Symptom Checker jako "educational content"
  - Disclaimer: "Not medical advice"
  - Zero personalization
  - Revenue: Booking marketplace (safe)

Phase 2 (Revenue Expansion): Non-device premium features
  - Appointment reminders
  - Clinic reviews
  - Telehealth infrastructure
  - Revenue: Subscription tiers

Phase 3 (Certification Complete): Medical features
  - AI Symptom Checker (certified)
  - Photo diagnosis
  - Risk prediction
  - Revenue: Premium AI features
```

**C) Parallel Track Strategy:**
```
Track A: EU certification (primary)
Track B: US market (FDA lower barrier)
  - FDA Digital Health Pre-Cert Program
  - "Breakthrough Device" designation
  - Faster approval (3-6 months)
  - Launch in US first if EU delays

Track C: Geographic arbitrage
  - India: No device approval needed
  - LatAm: Minimal requirements
  - Generate revenue while EU pending
```

**D) Escrow Dev Resources:**
```
Certification pending? → Freeze AI module code
Developers work on:
  - Telemedicine features
  - Marketplace improvements
  - Analytics dashboard
  - Platform stability

Post-certification: Quick deployment (code ready)
```

**Cost:** €10k pre-submission + opportunity cost (delayed revenue)
**Timeline:** Start Month 6 (6 months before planned submission)
**Fallback:** Launch without AI features, pivot to pure marketplace

---

#### **RISK #3: GDPR/HIPAA Compliance Breach**

**Severity:** 🔴 CRITICAL
**Probability:** Medium (data breaches = 30% startups w 3 years)
**Impact:** €20M fine (4% annual revenue) + reputational death

**Scenario:**
```
1. Developer accidentally logs PESEL (national ID) to CloudWatch
2. Logs exported to S3 (unencrypted)
3. S3 bucket misconfigured (public read)
4. Data scraped by bot → dark web
5. GDPR complaint filed
6. Investigation reveals: No DPO, no DPIA, no encryption
7. RESULT: €10M fine + forced shutdown
```

**Mitigation Strategies:**

**A) Privacy by Design Checklist:**
```yaml
# .github/workflows/privacy-check.yml
name: Privacy Compliance Check

on: [pull_request]

jobs:
  privacy-audit:
    runs-on: ubuntu-latest
    steps:
      - name: Check for PII in logs
        run: |
          # Fail if regex matches PESEL, email, phone
          if grep -rE '\b\d{11}\b|\b[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,}\b' src/; then
            echo "❌ PII detected in code!"
            exit 1
          fi

      - name: Verify encryption for sensitive fields
        run: |
          # Check Patient entity has encrypted fields
          if ! grep -q '@Encrypted' src/entities/patient.entity.ts; then
            echo "❌ Patient entity missing encryption!"
            exit 1
          fi

      - name: Check audit logging
        run: |
          # Verify all controllers have @UseInterceptors(AuditInterceptor)
          python scripts/verify_audit_coverage.py
```

**B) Automated PII Scrubbing:**
```typescript
// logger.service.ts
import { createLogger, format } from 'winston';

const piiRegex = {
  pesel: /\b\d{11}\b/g,
  email: /\b[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,}\b/gi,
  phone: /\b\d{3}[-.\s]?\d{3}[-.\s]?\d{3}\b/g,
};

const scrubPII = format((info) => {
  let message = JSON.stringify(info);

  // Replace all PII with [REDACTED]
  Object.entries(piiRegex).forEach(([type, regex]) => {
    message = message.replace(regex, `[REDACTED_${type.toUpperCase()}]`);
  });

  return JSON.parse(message);
});

export const logger = createLogger({
  format: format.combine(
    scrubPII(), // ← Always scrub before logging
    format.timestamp(),
    format.json()
  ),
});
```

**C) Data Protection Impact Assessment (DPIA):**
```markdown
# DPIA Template (EU GDPR Art. 35 requirement)

## Processing Activity: AI Symptom Checker

### Data Collected:
- Demographics: Age, sex, location
- Health data: Symptoms, medical history, photos
- Behavioral: App usage, search queries

### Legal Basis:
- Consent (GDPR Art. 6(1)(a) + Art. 9(2)(a) for health data)
- Legitimate interest (service improvement) - Art. 6(1)(f)

### Risks Identified:
1. Data breach → Patient harm (discrimination, identity theft)
2. AI bias → Incorrect medical advice → Patient harm
3. Unauthorized access → Privacy violation

### Safeguards:
1. Encryption at rest + transit (AES-256, TLS 1.3)
2. Access controls (RBAC, MFA for staff)
3. Regular penetration testing (quarterly)
4. Incident response plan (24h breach notification)
5. Data minimization (collect only necessary fields)
6. Anonymization for analytics (k-anonymity, l-diversity)

### DPO Sign-off: _______________  Date: _______________
```

**D) Hire Data Protection Officer (DPO):**
```
Full-time DPO: €60k/year (required if >250 employees OR high-risk processing)
  ↓
Alternative: Part-time DPO service (€1.5k/month)
  - Monthly compliance audits
  - DPIA reviews
  - Breach response
  - Regulator liaison

Cost: €18k/year vs €300k lawsuit
```

**E) Cyber Insurance:**
```
Coverage: €5M cyber liability
Premium: ~€8k/year
Covers:
  - Legal defense (GDPR complaints)
  - Breach notification costs
  - Credit monitoring for affected users
  - PR crisis management

ROI: €8k/year vs potential €10M+ exposure
```

**Cost:** €18k/year (DPO) + €8k/year (insurance) + 40h dev (automation) = €26k/year
**Timeline:** Before collecting any user data (Day 1)
**Fallback:** NONE - this is non-negotiable

---

#### **RISK #4: Multi-Tenancy Data Leakage**

**Severity:** 🔴 CRITICAL
**Probability:** Low (but catastrophic if happens)
**Impact:** Competitor clinic sees LuxMed patients → existential lawsuit

**Scenario:**
```
1. Tenant middleware fails to set search_path
2. Query executes against wrong schema (tenant_luxmed vs tenant_medicover)
3. Doctor from Medicover sees LuxMed patient list
4. Medicover steals patients, files lawsuit
5. GDPR breach + contract violation
6. RESULT: €50M lawsuit + platform shutdown
```

**Mitigation Strategies:**

**A) Defense in Depth (4 layers):**

**Layer 1: Middleware (primary protection):**
```typescript
// MUST set tenant on EVERY request
@Injectable()
export class TenantMiddleware implements NestMiddleware {
  use(req: Request, res: Response, next: NextFunction) {
    const tenantId = this.extractTenantId(req);

    if (!tenantId) {
      // NEVER allow requests without tenant
      throw new ForbiddenException('Missing tenant context');
    }

    req['tenantId'] = tenantId;
    next();
  }
}
```

**Layer 2: Database Row-Level Security (backup):**
```sql
-- Even if middleware fails, RLS blocks cross-tenant access
CREATE POLICY tenant_isolation ON appointments
  FOR ALL
  USING (
    tenant_id = current_setting('app.current_tenant')::UUID
  );

-- If tenant not set → RLS blocks ALL queries
```

**Layer 3: Application-level validation:**
```typescript
@Injectable()
export class AppointmentsService {
  async findOne(id: string, tenantId: string) {
    const appointment = await this.prisma.appointment.findFirst({
      where: {
        id,
        tenantId, // ← ALWAYS filter by tenant explicitly
      },
    });

    if (!appointment) {
      // Don't reveal if ID exists in other tenant
      throw new NotFoundException('Appointment not found');
    }

    return appointment;
  }
}
```

**Layer 4: Monitoring & Alerts:**
```typescript
// Detect cross-tenant queries
@Injectable()
export class TenantAuditInterceptor implements NestInterceptor {
  intercept(context: ExecutionContext, next: CallHandler) {
    const req = context.switchToHttp().getRequest();
    const requestTenant = req['tenantId'];

    return next.handle().pipe(
      tap((response) => {
        // Check if response contains data from wrong tenant
        if (Array.isArray(response)) {
          const foreignData = response.filter(
            item => item.tenantId !== requestTenant
          );

          if (foreignData.length > 0) {
            // 🚨 ALERT: Data leakage detected!
            this.alertService.critical('TENANT_LEAK', {
              requestTenant,
              leakedTenants: foreignData.map(d => d.tenantId),
              endpoint: req.url,
            });

            // Filter out foreign data before returning
            return response.filter(item => item.tenantId === requestTenant);
          }
        }
      })
    );
  }
}
```

**B) Penetration Testing:**
```bash
# Test script: Try to access other tenant's data
curl -H "X-Tenant-ID: luxmed" \
     -H "Authorization: Bearer $MEDICOVER_DOCTOR_TOKEN" \
     https://api.yourmedic.pl/appointments

# Expected: 403 Forbidden
# If 200 OK → CRITICAL BUG
```

**C) Tenant Isolation Test Suite:**
```typescript
// tests/tenant-isolation.e2e-spec.ts
describe('Tenant Isolation (Security)', () => {
  it('should block cross-tenant appointment access', async () => {
    // Doctor from Medicover
    const medicover_token = await authenticate('medicover_doctor');

    // Try to access LuxMed appointment
    const response = await request(app.getHttpServer())
      .get('/appointments/luxmed-appointment-id-123')
      .set('Authorization', `Bearer ${medicover_token}`)
      .set('X-Tenant-ID', 'medicover');

    expect(response.status).toBe(404); // Not 200!
  });

  it('should prevent SQL injection to change tenant', async () => {
    const response = await request(app.getHttpServer())
      .get('/appointments')
      .set('X-Tenant-ID', "medicover'; SET search_path TO tenant_luxmed; --");

    expect(response.status).toBe(400); // Reject malformed tenant ID
  });
});
```

**Cost:** 60h dev (RLS + monitoring) + €5k/year penetration testing
**Timeline:** Before first multi-tenant deployment
**Fallback:** Database-per-tenant (expensive but foolproof isolation)

---

#### **RISK #5: AI/ML Model Bias & Discrimination**

**Severity:** 🟠 HIGH
**Probability:** Medium (bias exists in 60% medical AI models)
**Impact:** Lawsuit + regulatory action + harm to patients

**Scenario:**
```
1. AI Symptom Checker trained on data from urban Polish clinics
2. Dataset: 80% young, 15% middle-age, 5% elderly
3. Model underperforms for elderly patients
4. 70-year-old woman gets "low priority" for heart attack symptoms
5. She delays seeking care → dies
6. Family sues for discrimination + negligence
7. RESULT: €10M lawsuit + criminal charges + platform ban
```

**Mitigation Strategies:**

**A) Bias Detection in Training Pipeline:**
```python
# ml_training/bias_detection.py
from aequitas.group import Group
from aequitas.bias import Bias

def detect_bias(model, test_data):
    """
    Check model performance across demographic groups
    """
    predictions = model.predict(test_data)

    # Create bias report
    g = Group()
    xtab, _ = g.get_crosstabs(test_data, predictions)

    b = Bias()
    bias_df = b.get_disparity_predefined_groups(
        xtab,
        original_df=test_data,
        ref_groups_dict={
            'age': 'middle',  # Reference group
            'sex': 'male',
            'location': 'urban',
        }
    )

    # Check if any group has <80% accuracy vs reference (80% rule)
    for group in bias_df.itertuples():
        if group.accuracy_disparity < 0.8:
            print(f"⚠️ BIAS DETECTED: {group.attribute_name} = {group.attribute_value}")
            print(f"   Accuracy: {group.accuracy:.2%} vs {group.ref_accuracy:.2%}")
            raise ValueError("Model fails fairness threshold")

    return bias_df

# Run before deployment
if __name__ == '__main__':
    model = load_model('symptom_checker_v2.1.h5')
    test_data = load_test_data('data/test_diverse.csv')

    bias_report = detect_bias(model, test_data)
    bias_report.to_csv('reports/bias_audit.csv')
```

**B) Diverse Training Data Collection:**
```
Problem: Polish clinic data = urban, young, affluent

Solution: Partner with diverse clinics
  - Rural health centers (older population)
  - Public hospitals (diverse socioeconomic)
  - Specialist clinics (chronic conditions)

Target Demographics:
  Age: 20% <30, 40% 30-50, 30% 50-70, 10% >70
  Sex: 50/50
  Location: 60% urban, 40% rural
  Conditions: Common (70%) + Rare (30%)

Cost: €20k incentives for data sharing
```

**C) Confidence Thresholds per Demographic:**
```python
# Adaptive confidence based on group representation
def get_confidence_threshold(patient_age, patient_sex):
    """
    Lower threshold for underrepresented groups
    (Better to say "I don't know" than give bad advice)
    """
    thresholds = {
        'default': 0.75,
        'elderly': 0.85,  # Higher bar (less training data)
        'rare_condition': 0.90,
    }

    if patient_age > 65:
        return thresholds['elderly']
    else:
        return thresholds['default']

# In prediction endpoint
prediction_confidence = model.predict_proba(features).max()
threshold = get_confidence_threshold(patient.age, patient.sex)

if prediction_confidence < threshold:
    return {
        "result": "UNCERTAIN",
        "message": "Our AI cannot confidently assess your symptoms. Please consult a doctor.",
        "recommended_action": "URGENT_CARE"
    }
```

**D) Explainable AI (XAI) dla Audits:**
```python
import shap

# Generate SHAP explanations for every prediction
explainer = shap.TreeExplainer(model)
shap_values = explainer.shap_values(patient_features)

# Log explanation for audit trail
audit_log = {
    "patient_id": patient_id,
    "prediction": prediction,
    "confidence": confidence,
    "feature_importance": {
        "symptom_fever": shap_values[0][0],
        "symptom_cough": shap_values[0][1],
        "age": shap_values[0][2],
        # ... all features
    },
    "human_readable": f"Decision driven by: {top_3_features}"
}

# If lawsuit → Can prove decision was not based on age/sex
```

**E) Human Oversight Requirement:**
```
AI Classification:
  - LOW risk → Patient books GP appointment (automated)
  - MEDIUM risk → Suggest specialist (automated)
  - HIGH risk → Flag for human review (doctor triages within 2h)
  - CRITICAL risk → Emergency alert (call ambulance immediately)

High-risk groups (elderly, chronic conditions):
  - ALWAYS escalate to human review
  - Never fully automated
```

**Cost:** €20k data collection + 40h bias detection + €30k diverse dataset
**Timeline:** Before AI certification submission
**Fallback:** Don't launch AI for high-risk demographics (segment by age)

---

#### **RISK #6: Backend Scaling Bottleneck**

**Severity:** 🟡 MEDIUM
**Probability:** High (90% startups underestimate growth)
**Impact:** Platform downtime during viral growth → user churn

**Scenario:**
```
1. Launch MVP: 1,000 users, NestJS single instance (t3.medium)
2. Viral TikTok → 50,000 users signup in 1 week
3. Database connections exhausted (max 100 PostgreSQL)
4. API requests timeout
5. Users see errors → 1-star App Store reviews
6. Growth stalls → momentum lost
7. RESULT: Missed opportunity window
```

**Mitigation Strategies:**

**A) Connection Pooling + Read Replicas:**
```typescript
// database.module.ts
import { TypeOrmModule } from '@nestjs/typeorm';

@Module({
  imports: [
    TypeOrmModule.forRoot({
      type: 'postgres',
      host: process.env.DB_HOST,
      port: 5432,

      // Connection pooling (prevent exhaustion)
      extra: {
        max: 20, // Max connections per instance
        min: 5,  // Keep warm pool
        idleTimeoutMillis: 30000,
        connectionTimeoutMillis: 2000,
      },

      // Read replicas for scaling reads
      replication: {
        master: {
          host: process.env.DB_MASTER_HOST,
          port: 5432,
        },
        slaves: [
          { host: process.env.DB_REPLICA_1_HOST, port: 5432 },
          { host: process.env.DB_REPLICA_2_HOST, port: 5432 },
        ],
      },
    }),
  ],
})
export class DatabaseModule {}

// Usage: Queries auto-routed to replicas
const patients = await this.patientRepository.find(); // ← Hits replica
await this.patientRepository.save(patient); // ← Hits master
```

**B) Redis Caching Strategy:**
```typescript
// caching.service.ts
@Injectable()
export class CachingService {
  constructor(@Inject(CACHE_MANAGER) private cache: Cache) {}

  async getCachedOrFetch<T>(
    key: string,
    fetchFn: () => Promise<T>,
    ttl: number = 3600 // 1 hour default
  ): Promise<T> {
    // Check cache first
    const cached = await this.cache.get<T>(key);
    if (cached) return cached;

    // Cache miss → Fetch from DB
    const data = await fetchFn();
    await this.cache.set(key, data, { ttl });
    return data;
  }
}

// appointments.service.ts
async getDoctorSchedule(doctorId: string, date: Date) {
  const cacheKey = `doctor:${doctorId}:schedule:${date.toISOString()}`;

  return this.cachingService.getCachedOrFetch(
    cacheKey,
    () => this.fetchScheduleFromDB(doctorId, date),
    3600 // Cache for 1 hour
  );
}
```

**C) Auto-Scaling Infrastructure (AWS ECS Fargate):**
```yaml
# infrastructure/ecs-service.yml
Resources:
  YourMedicService:
    Type: AWS::ECS::Service
    Properties:
      Cluster: !Ref ECSCluster
      TaskDefinition: !Ref TaskDefinition
      DesiredCount: 2 # Start with 2 instances

      # Auto-scaling based on CPU/Memory
      AutoScalingTarget:
        MinCapacity: 2
        MaxCapacity: 50 # Can scale to 50 instances
        TargetCPUUtilization: 70 # Scale up if CPU >70%
        TargetMemoryUtilization: 80

      # Scale based on request count
      TargetTrackingScaling:
        - MetricName: RequestCountPerTarget
          TargetValue: 1000 # 1000 req/min per instance
```

**D) Database Sharding dla Long-term:**
```sql
-- Horizontal partitioning by tenant_id
CREATE TABLE appointments_partition_0
  PARTITION OF appointments
  FOR VALUES WITH (MODULUS 4, REMAINDER 0);

CREATE TABLE appointments_partition_1
  PARTITION OF appointments
  FOR VALUES WITH (MODULUS 4, REMAINDER 1);

-- Queries automatically routed to correct partition
-- SELECT * FROM appointments WHERE tenant_id = 'luxmed'
-- → Only scans appointments_partition_2 (25% of data)
```

**E) Load Testing BEFORE Launch:**
```bash
# k6 load test script
import http from 'k6/http';
import { check, sleep } from 'k6';

export let options = {
  stages: [
    { duration: '2m', target: 100 },   // Ramp up to 100 users
    { duration: '5m', target: 100 },   // Stay at 100
    { duration: '2m', target: 1000 },  // Spike to 1000
    { duration: '5m', target: 1000 },  // Hold spike
    { duration: '2m', target: 0 },     // Ramp down
  ],
  thresholds: {
    http_req_duration: ['p(95)<500'], // 95% requests <500ms
    http_req_failed: ['rate<0.01'],   // <1% error rate
  },
};

export default function () {
  const res = http.get('https://api.yourmedic.pl/appointments');
  check(res, {
    'status is 200': (r) => r.status === 200,
    'response time < 500ms': (r) => r.timings.duration < 500,
  });
  sleep(1);
}
```

**Cost:** €200/month (read replicas + Redis) + €500/month (Fargate auto-scaling reserve)
**Timeline:** Before public beta launch
**Fallback:** Waitlist (control growth rate) + scaling up manually

---

**💎 KEY INSIGHTS Branch 4 (Technical Risks):**
> **Offline Conflicts:** CRDT + Operational Transform + Conflict UI (never silent data loss)
> **Certification:** Pre-submission consultation (Month 6), parallel US/EU tracks, phased features (MVP = no medical device)
> **GDPR:** Privacy by design (PII scrubbing, DPO, DPIA, cyber insurance €26k/year), defense in depth
> **Multi-tenancy:** 4-layer isolation (middleware + RLS + app validation + monitoring), quarterly pentesting
> **AI Bias:** Diverse training data (€20k), bias detection pipeline (80% rule), adaptive confidence, human oversight for high-risk
> **Scaling:** Read replicas + Redis + auto-scaling (2-50 instances), load testing BEFORE launch

**━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━**

### **Branch 5: Success Metrics & KPIs**

**Framework:** OKRs (Objectives & Key Results) + North Star Metric

---

#### **NORTH STAR METRIC**

**Metric:** Monthly Active Appointments Completed (MAAC)

**Rationale:**
```
Why not MAU (Monthly Active Users)?
  → Users can browse but not book = no value delivered

Why not Revenue?
  → Early stage = growth > profit

Why Appointments Completed?
  ✅ Measures real value delivery (patient got care)
  ✅ Aligns all 3 user groups (Patient + Doctor + Clinic)
  ✅ Leading indicator of revenue (commission per appointment)
  ✅ Compounding network effect (more doctors → more patients → more doctors)
```

**Target Trajectory:**
```
Month 3 (Private Beta):     100 MAAC
Month 6 (Public Launch):  1,000 MAAC  (10x)
Month 12:                10,000 MAAC  (10x)
Month 24:               100,000 MAAC  (10x)
Month 36:             1,000,000 MAAC  (sustainable growth 2-3x/year)
```

**Breakdown by User Type:**
```
Patients:  60% new, 40% returning (retention critical)
Doctors:   20% on platform actively booking (activation key)
Clinics:   Average 50 appointments/month per clinic
```

---

#### **CATEGORY 1: User Growth Metrics**

**Objective:** Build sustainable user acquisition loops across all 3 sides of marketplace

---

**1A) Patient Acquisition**

**KPI:** Cost Per Acquired Patient (CPAP)
```
Target: <€5 per signup (organic + paid)
Benchmark: Docplanner (€15-20), ZnanyLekarz (€10-15)

Channels:
  - Organic (Google "dentysta Warszawa"): €0 (SEO)
  - Social (TikTok, Instagram): €3-5 (viral content)
  - Paid (Google Ads): €8-12 (retargeting existing intent)
  - Referral: €0.50 (€5 credit to referrer)
```

**Measurement:**
```sql
SELECT
  acquisition_channel,
  COUNT(DISTINCT user_id) AS signups,
  SUM(marketing_spend) AS total_cost,
  SUM(marketing_spend) / COUNT(DISTINCT user_id) AS cpap
FROM patient_acquisitions
WHERE signup_date >= DATE_TRUNC('month', CURRENT_DATE)
GROUP BY acquisition_channel;
```

**Success Threshold:**
- CPAP < €5 → GREEN (sustainable)
- CPAP €5-10 → YELLOW (monitor closely)
- CPAP > €10 → RED (unprofitable, adjust strategy)

---

**1B) Doctor Activation Rate**

**KPI:** % of registered doctors who complete first appointment within 30 days
```
Target: 40% activation rate
Industry: 15-25% (we need to be 2x better)

Activation = Doctor completes:
  1. Profile setup (photo, bio, specialization)
  2. Availability calendar (min 10 slots/week)
  3. First appointment booked + completed
```

**Cohort Analysis:**
```typescript
// analytics/doctor-activation.ts
interface ActivationFunnel {
  registered: number;
  profileCompleted: number;
  calendarSet: number;
  firstAppointment: number;
}

async function getDoctorActivationCohort(monthYear: string) {
  const cohort = await db.query(`
    SELECT
      COUNT(*) AS registered,
      COUNT(CASE WHEN profile_completed_at IS NOT NULL THEN 1 END) AS profile_completed,
      COUNT(CASE WHEN calendar_set_at IS NOT NULL THEN 1 END) AS calendar_set,
      COUNT(CASE WHEN first_appointment_at <= registered_at + INTERVAL '30 days' THEN 1 END) AS first_appointment
    FROM doctors
    WHERE DATE_TRUNC('month', registered_at) = $1
  `, [monthYear]);

  return {
    ...cohort,
    activationRate: (cohort.first_appointment / cohort.registered) * 100
  };
}
```

**Drop-off Points (typical):**
- Registered → Profile: 70% (30% drop)
- Profile → Calendar: 60% (10% drop)
- Calendar → First Appointment: 40% (20% drop)

**Interventions:**
```
If activation < 30%:
  → Week 1: Email drip campaign (setup guide)
  → Week 2: SMS reminder + personal call (support team)
  → Week 3: "Limited slots available" urgency
  → Week 4: Temporary profile visibility boost (free marketing)
```

---

**1C) Clinic Onboarding Speed**

**KPI:** Time from clinic signup → first 100 appointments
```
Target: <60 days
Benchmark: Docplanner (90-120 days)

Breakdown:
  - Day 1-7:   Sales demo + contract signed
  - Day 8-14:  Integration setup (FHIR/CSV import)
  - Day 15-21: Doctor training (5-10 doctors/clinic)
  - Day 22-30: Soft launch (internal testing)
  - Day 31-60: Ramp to 100 appointments (marketing push)
```

**Dashboard:**
```typescript
// Clinic onboarding health dashboard
interface ClinicOnboardingMetrics {
  clinicId: string;
  clinicName: string;
  daysS inceSignup: number;
  currentStage: 'contract' | 'integration' | 'training' | 'soft_launch' | 'live';
  doctorsOnboarded: number;
  appointmentsCompleted: number;
  daysTo100Appointments: number | null; // null if not reached
  healthStatus: 'on_track' | 'at_risk' | 'churned';
}

function calculateHealthStatus(clinic: ClinicOnboardingMetrics): string {
  if (clinic.daysTo100Appointments && clinic.daysTo100Appointments <= 60) {
    return 'on_track';
  } else if (clinic.daysSinceSignup > 90 && clinic.appointmentsCompleted < 50) {
    return 'churned'; // Likely won't activate
  } else {
    return 'at_risk'; // Needs intervention
  }
}
```

---

#### **CATEGORY 2: Engagement & Retention Metrics**

**Objective:** Turn one-time users into habitual users (weekly/monthly engagement)

---

**2A) Patient Retention (Cohort Analysis)**

**KPI:** Month N Retention Rate
```
Target:
  - M1 (1 month later):  40% return
  - M3 (3 months later): 25% return
  - M6 (6 months later): 15% return

Benchmark: Docplanner (M1: 30%, M3: 18%, M6: 10%)
```

**Retention Curve:**
```
100% ┤
     │ ●
     │   ●●
 60% │     ●●
     │       ●●
 40% │ ────────●●────── M1 Target (40%)
     │           ●●●
 25% │ ──────────────●●● M3 Target (25%)
     │               ●●●
 15% │ ──────────────────●● M6 Target (15%)
  0% └───────────────────────●●●●●●●
     M0  M1  M2  M3  M4  M5  M6
```

**SQL Query:**
```sql
WITH cohorts AS (
  SELECT
    user_id,
    DATE_TRUNC('month', first_appointment_date) AS cohort_month
  FROM patients
),
retention AS (
  SELECT
    c.cohort_month,
    COUNT(DISTINCT c.user_id) AS cohort_size,
    COUNT(DISTINCT CASE
      WHEN a.appointment_date >= c.cohort_month + INTERVAL '1 month'
       AND a.appointment_date < c.cohort_month + INTERVAL '2 months'
      THEN c.user_id
    END) AS m1_retained,
    COUNT(DISTINCT CASE
      WHEN a.appointment_date >= c.cohort_month + INTERVAL '3 months'
       AND a.appointment_date < c.cohort_month + INTERVAL '4 months'
      THEN c.user_id
    END) AS m3_retained
  FROM cohorts c
  LEFT JOIN appointments a ON c.user_id = a.patient_id
  GROUP BY c.cohort_month
)
SELECT
  cohort_month,
  cohort_size,
  ROUND(100.0 * m1_retained / cohort_size, 2) AS m1_retention_pct,
  ROUND(100.0 * m3_retained / cohort_size, 2) AS m3_retention_pct
FROM retention
ORDER BY cohort_month DESC;
```

**Retention Triggers (automated):**
```typescript
// Trigger: Patient hasn't booked in 60 days
@Cron('0 9 * * *') // Daily at 9 AM
async sendRetentionCampaign() {
  const dormantPatients = await this.db.query(`
    SELECT user_id, email, last_appointment_date
    FROM patients
    WHERE last_appointment_date < CURRENT_DATE - INTERVAL '60 days'
      AND last_appointment_date > CURRENT_DATE - INTERVAL '65 days'
  `);

  for (const patient of dormantPatients) {
    await this.emailService.send({
      to: patient.email,
      template: 'retention_60day',
      data: {
        patientName: patient.name,
        incentive: '20% discount on next appointment',
        cta: 'Book your check-up now',
      },
    });
  }
}
```

---

**2B) Doctor Utilization Rate**

**KPI:** % of available slots actually booked
```
Target: 60% utilization
Industry: 40-50%

Formula:
Utilization = (Booked Slots / Available Slots) * 100

Example:
  - Doctor sets 40 slots/week (8 hours/day, 30min slots)
  - 24 slots booked
  - Utilization = 24/40 = 60% ✅
```

**Why this matters:**
```
High utilization (>80%):
  ✅ Doctor is making money
  ❌ Risk of burnout
  ❌ No slots for urgent patients
  → Action: Suggest adding more availability

Low utilization (<30%):
  ❌ Doctor wasting time
  ❌ Platform not delivering value
  → Action: Boost profile visibility, reduce pricing
```

**Doctor Dashboard:**
```typescript
// Real-time utilization widget
interface DoctorUtilizationWidget {
  thisWeek: {
    availableSlots: 40;
    bookedSlots: 24;
    utilization: 60;
    status: 'healthy'; // 'healthy' | 'low' | 'high'
  };
  lastWeek: {
    utilization: 55;
    trend: '+5%'; // vs last week
  };
  suggestions: [
    'Add 2 more evening slots (highest demand)',
    'Reduce Friday afternoon slots (low bookings)'
  ];
}
```

---

**2C) Session Duration & Feature Usage**

**KPI:** Average session duration + feature engagement
```
Patients:
  - Avg session: 4-6 minutes
  - Pages per session: 3-5
  - Key flow: Search → Profile → Book (conversion funnel)

Doctors:
  - Avg session: 8-12 minutes
  - Daily logins: 2-3 (morning check + evening notes)
  - Key features: Calendar (80% usage), Patient notes (60%), Chat (40%)

Clinics (Admin):
  - Avg session: 15-20 minutes
  - Weekly logins: 5-7
  - Key features: Analytics dashboard (90%), Doctor management (70%), Billing (100%)
```

**Feature Adoption Tracking:**
```typescript
// Track which features drive retention
interface FeatureUsageCorrelation {
  feature: string;
  usersWhoUsed: number;
  m3RetentionRate: number;
  correlationCoefficient: number; // -1 to 1
}

// Example results:
const featureImpact = [
  { feature: 'AI Symptom Checker', usersWhoUsed: 12000, m3RetentionRate: 45, correlation: 0.78 },
  { feature: 'Appointment Reminders', usersWhoUsed: 30000, m3RetentionRate: 38, correlation: 0.62 },
  { feature: 'Telehealth', usersWhoUsed: 8000, m3RetentionRate: 52, correlation: 0.85 },
  { feature: 'Wearables Sync', usersWhoUsed: 3000, m3RetentionRate: 61, correlation: 0.92 }, // ← Power user feature!
];

// Insight: Users who sync wearables have 2.4x retention!
// Action: Promote wearables integration to all users
```

---

#### **CATEGORY 3: Quality & Healthcare Outcomes**

**Objective:** Ensure platform delivers high-quality healthcare experiences (not just bookings)

---

**3A) Patient Satisfaction (NPS)**

**KPI:** Net Promoter Score
```
Target: NPS > 50 (world-class)
Industry: 20-40 (healthcare platforms)

NPS Calculation:
  - Survey: "How likely are you to recommend YourMedic?" (0-10)
  - Promoters (9-10):  X%
  - Passives (7-8):    Y%
  - Detractors (0-6):  Z%
  - NPS = Promoters% - Detractors%

Example:
  50% promoters, 30% passives, 20% detractors
  NPS = 50 - 20 = 30
```

**Survey Timing:**
```typescript
// Trigger NPS survey 24h after appointment
@Cron('0 10 * * *') // Daily at 10 AM
async sendNPSSurveys() {
  const completedAppointments = await this.db.query(`
    SELECT a.id, a.patient_id, p.email
    FROM appointments a
    JOIN patients p ON a.patient_id = p.id
    WHERE a.completed_at = CURRENT_DATE - INTERVAL '1 day'
      AND a.nps_survey_sent = FALSE
  `);

  for (const apt of completedAppointments) {
    await this.emailService.send({
      to: apt.email,
      template: 'nps_survey',
      data: {
        appointmentId: apt.id,
        surveyLink: `https://yourmedic.pl/survey/${apt.id}`,
      },
    });

    // Mark as sent
    await this.db.query(`
      UPDATE appointments
      SET nps_survey_sent = TRUE
      WHERE id = $1
    `, [apt.id]);
  }
}
```

**Detractor Follow-up:**
```typescript
// Auto-escalate detractors (score 0-6) to support team
async handleNPSResponse(appointmentId: string, score: number, comment: string) {
  if (score <= 6) {
    // Create support ticket
    await this.supportService.createTicket({
      priority: 'high',
      category: 'patient_dissatisfaction',
      appointmentId,
      comment,
      assignedTo: 'customer_success_team',
    });

    // Send personalized email
    await this.emailService.send({
      to: patient.email,
      from: 'support@yourmedic.pl',
      subject: 'We want to make things right',
      body: `Hi ${patient.name}, we're sorry your experience wasn't perfect...`,
    });
  }
}
```

---

**3B) Appointment No-Show Rate**

**KPI:** % of booked appointments where patient doesn't show up
```
Target: <5% no-show rate
Industry: 15-30% (massive problem in healthcare)

Why it matters:
  - Doctor wasted time = lost revenue
  - Slot could have gone to another patient
  - Clinic efficiency drops
```

**No-show Prevention:**
```typescript
// Multi-touchpoint reminder system
async scheduleReminders(appointmentId: string) {
  const appointment = await this.getAppointment(appointmentId);

  // Reminder 1: 24 hours before
  await this.scheduledTasksService.schedule({
    executeAt: appointment.startTime.minus({ hours: 24 }),
    task: 'send_sms_reminder',
    payload: { appointmentId, message: 'Jutro masz wizytę o ${time}. Potwierdź klikając link.' },
  });

  // Reminder 2: 2 hours before
  await this.scheduledTasksService.schedule({
    executeAt: appointment.startTime.minus({ hours: 2 }),
    task: 'send_push_notification',
    payload: { appointmentId, message: 'Za 2 godziny wizyta. Pamiętaj!' },
  });

  // Reminder 3: 30 min before (with Maps directions)
  await this.scheduledTasksService.schedule({
    executeAt: appointment.startTime.minus({ minutes: 30 }),
    task: 'send_navigation_prompt',
    payload: {
      appointmentId,
      clinicAddress: appointment.clinic.address,
      mapsLink: `https://maps.google.com/?q=${appointment.clinic.lat},${appointment.clinic.lng}`,
    },
  });
}
```

**No-show Consequences:**
```typescript
// Penalize repeat no-shows
async handleNoShow(appointmentId: string) {
  const patient = await this.getPatientFromAppointment(appointmentId);
  const noShowCount = await this.getNoShowCount(patient.id, '90 days');

  if (noShowCount === 1) {
    // Warning
    await this.emailService.send({
      to: patient.email,
      template: 'noshow_warning',
      message: 'Please cancel in advance if you can\'t make it.',
    });
  } else if (noShowCount === 2) {
    // Require prepayment for future bookings
    await this.db.query(`
      UPDATE patients
      SET requires_prepayment = TRUE
      WHERE id = $1
    `, [patient.id]);
  } else if (noShowCount >= 3) {
    // Temporary booking restriction (30 days)
    await this.db.query(`
      UPDATE patients
      SET booking_restricted_until = CURRENT_DATE + INTERVAL '30 days'
      WHERE id = $1
    `, [patient.id]);
  }
}
```

---

**3C) Average Wait Time (Appointment → Actual Visit)**

**KPI:** Days from booking to appointment date
```
Target: <7 days average wait time
Industry: 14-30 days (Poland)

Breakdown by specialty:
  - GP (General Practitioner): <3 days
  - Specialist (Dermatologist, etc): <7 days
  - Urgent care: Same day / Next day
```

**Why it matters:**
```
Long wait times:
  ❌ Patient health deteriorates (medical risk)
  ❌ Patient books elsewhere (churn)
  ❌ Poor marketplace liquidity (supply/demand imbalance)

Short wait times:
  ✅ Better health outcomes
  ✅ Higher patient satisfaction
  ✅ Network effect (patients refer friends)
```

**Supply/Demand Balancing:**
```typescript
// Alert when wait times spike
@Cron('0 8 * * 1') // Every Monday 8 AM
async analyzeWaitTimes() {
  const waitTimes = await this.db.query(`
    SELECT
      d.specialization,
      AVG(EXTRACT(EPOCH FROM (a.appointment_date - a.booked_at)) / 86400) AS avg_wait_days,
      COUNT(*) AS total_bookings
    FROM appointments a
    JOIN doctors d ON a.doctor_id = d.id
    WHERE a.booked_at >= CURRENT_DATE - INTERVAL '7 days'
    GROUP BY d.specialization
  `);

  for (const specialty of waitTimes) {
    if (specialty.avg_wait_days > 7) {
      // Alert: Need more doctors in this specialty
      await this.alertService.send({
        channel: 'slack',
        message: `⚠️ ${specialty.specialization} wait time: ${specialty.avg_wait_days} days (target: <7)`,
        action: `Recruit more ${specialty.specialization} doctors or incentivize existing ones to add more slots`,
      });
    }
  }
}
```

---

#### **CATEGORY 4: Revenue & Business Metrics**

**Objective:** Build sustainable, profitable business model

---

**4A) Monthly Recurring Revenue (MRR)**

**KPI:** Predictable monthly revenue from subscriptions + commissions
```
Target Trajectory:
  Month 6:  €10,000 MRR
  Month 12: €50,000 MRR
  Month 24: €250,000 MRR

Revenue Streams:
  1. Marketplace commission (15% of appointment fee)
     - Example: €50 appointment → €7.50 to YourMedic
     - Target: 10,000 appointments/month = €75,000 commission revenue

  2. Clinic subscriptions (B2B SaaS)
     - Basic: €299/month (1 clinic, 10 doctors, booking only)
     - Pro: €799/month (analytics, custom branding, priority support)
     - Enterprise: €1,999/month (API access, white-label, dedicated success manager)
     - Target: 50 clinics @ €799 avg = €40,000 subscription revenue

  3. Premium patient features (freemium)
     - AI Symptom Checker Pro: €4.99/month
     - Wearables integration: €2.99/month
     - Priority booking: €9.99/month
     - Target: 5% conversion (500 users @ €5 avg) = €2,500 premium revenue

Total MRR = €75k + €40k + €2.5k = €117,500
```

**MRR Growth Rate:**
```typescript
interface MRRMetrics {
  currentMRR: number;
  newMRR: number;        // New customers
  expansionMRR: number;  // Upgrades (Basic → Pro)
  contractionMRR: number; // Downgrades (Pro → Basic)
  churnedMRR: number;    // Cancelled subscriptions
  netNewMRR: number;     // newMRR + expansionMRR - contractionMRR - churnedMRR
  mrrGrowthRate: number; // (netNewMRR / currentMRR) * 100
}

// Example:
const month6 = {
  currentMRR: 50000,
  newMRR: 12000,         // 15 new clinics @ €799
  expansionMRR: 3000,    // 5 clinics upgraded to Pro
  contractionMRR: 800,   // 2 clinics downgraded
  churnedMRR: 1200,      // 1.5 clinics cancelled
  netNewMRR: 13000,      // 12k + 3k - 0.8k - 1.2k
  mrrGrowthRate: 26,     // 26% MoM growth
};

// Healthy SaaS: 10-20% MoM growth (early stage)
// Target: 20%+ in first year, then stabilize to 10%
```

---

**4B) Customer Acquisition Cost (CAC) vs Lifetime Value (LTV)**

**KPI:** LTV:CAC Ratio
```
Target: LTV:CAC > 3:1
Industry: 3:1 to 5:1 (sustainable SaaS)

CAC Calculation:
  Total Sales & Marketing Spend / New Customers Acquired

Example:
  €30,000 marketing spend in Month 6
  500 new patients, 10 new clinics acquired
  Patient CAC = €30k / 500 = €60
  Clinic CAC = €30k / 10 = €3,000 (includes sales team)

LTV Calculation:
  Average Revenue Per User (ARPU) × Customer Lifetime

Example (Patient):
  ARPU = €7.50 commission per appointment
  Avg 2 appointments/year
  Avg customer lifetime = 3 years
  LTV = €7.50 × 2 × 3 = €45

  LTV:CAC = €45 / €60 = 0.75:1 ❌ UNPROFITABLE!

Example (Clinic):
  ARPU = €799/month subscription
  Avg customer lifetime = 2 years (24 months)
  LTV = €799 × 24 = €19,176

  LTV:CAC = €19,176 / €3,000 = 6.4:1 ✅ HIGHLY PROFITABLE!
```

**Insight:**
```
Clinic B2B model > Patient B2C model (for profitability)

Strategy:
  - Focus sales team on clinic acquisition (high LTV)
  - Use organic/viral for patient acquisition (reduce CAC to €10-20)
  - Cross-sell: Acquire patients through clinics (€0 CAC via referrals)
```

---

**4C) Churn Rate**

**KPI:** Monthly Revenue Churn %
```
Target: <5% monthly churn (SaaS benchmark)
Healthcare: 3-7% (sticky due to switching costs)

Formula:
Monthly Churn % = (Churned MRR / Beginning MRR) × 100

Example:
  Beginning MRR: €50,000
  Churned MRR: €1,500 (2 clinics cancelled)
  Monthly Churn = (€1,500 / €50,000) × 100 = 3% ✅
```

**Churn Analysis:**
```typescript
// Identify churn patterns
interface ChurnAnalysis {
  segment: string;
  churnRate: number;
  topReasons: Array<{ reason: string; percentage: number }>;
  lifetimeValue: number;
}

const churnData: ChurnAnalysis[] = [
  {
    segment: 'Small clinics (1-5 doctors)',
    churnRate: 8,
    topReasons: [
      { reason: 'Not enough bookings', percentage: 60 },
      { reason: 'Too expensive', percentage: 25 },
      { reason: 'Switched to competitor', percentage: 15 },
    ],
    lifetimeValue: 4800, // €799 × 6 months avg
  },
  {
    segment: 'Medium clinics (6-20 doctors)',
    churnRate: 3,
    topReasons: [
      { reason: 'Integration issues', percentage: 50 },
      { reason: 'Missing features', percentage: 30 },
      { reason: 'Support quality', percentage: 20 },
    ],
    lifetimeValue: 19176, // €799 × 24 months avg
  },
];

// Action: Focus retention efforts on Medium clinics (higher LTV, lower churn)
```

**Churn Prevention (Proactive):**
```typescript
// Predict churn using engagement signals
async identifyAtRiskClinics() {
  const atRisk = await this.db.query(`
    SELECT
      c.id,
      c.name,
      COUNT(a.id) AS appointments_last_30d,
      u.last_login_at,
      EXTRACT(DAY FROM CURRENT_DATE - u.last_login_at) AS days_since_login
    FROM clinics c
    JOIN users u ON c.admin_user_id = u.id
    LEFT JOIN appointments a ON c.id = a.clinic_id
      AND a.created_at >= CURRENT_DATE - INTERVAL '30 days'
    GROUP BY c.id, c.name, u.last_login_at
    HAVING
      COUNT(a.id) < 10  -- Low usage
      OR EXTRACT(DAY FROM CURRENT_DATE - u.last_login_at) > 14  -- Not logging in
  `);

  for (const clinic of atRisk) {
    // Trigger intervention
    await this.customerSuccessService.scheduleCall({
      clinicId: clinic.id,
      urgency: 'high',
      script: 'churn_prevention',
      goal: 'Identify blockers and re-engage',
    });
  }
}
```

---

**💎 KEY INSIGHTS Branch 5 (Success Metrics):**
> **North Star:** Monthly Active Appointments Completed (MAAC) - aligns value delivery across all 3 user types
> **Growth:** CPAP <€5 (beat competitors by 2-3x), Doctor activation 40% (2x industry), Clinic onboarding <60 days
> **Engagement:** Patient M3 retention 25%, Doctor utilization 60%, Feature correlation tracking (wearables = 2.4x retention!)
> **Quality:** NPS >50 (world-class), No-show <5% (vs industry 15-30%), Wait time <7 days (vs 14-30)
> **Revenue:** €117k MRR target (Month 12), LTV:CAC >3:1 (Clinics 6.4:1 profitable, Patients optimize to 3:1), Churn <5%
> **Strategy:** B2B (Clinics) = profit engine, B2C (Patients) = volume/growth engine, Cross-sell = €0 CAC goldmine

---

## 🔮 Technique 2: What If Scenarios

**Duration:** 15-20 minutes
**Goal:** Explore radical possibilities, extreme scenarios, and breakthrough opportunities

### **Category A: Wildly Optimistic Scenarios**

---

#### **SCENARIO 1: What if YourMedic goes viral on TikTok/Instagram?**

**Trigger:**
- Influencer shares story: "Znalazłam dermatologa w 24h dzięki YourMedic!"
- Video gets 5M views in 48 hours
- 200,000 signups in one week

**Implications:**
```
Opportunities:
✅ Massive user base = network effect kicks in
✅ Press coverage (Forbes, TechCrunch)
✅ VC interest spikes (Series A at higher valuation)
✅ Doctor FOMO → easier recruitment

Challenges:
❌ Infrastructure crash (not ready for 200k users)
❌ Customer support overwhelmed (1 person → 5,000 tickets)
❌ Doctor supply shortage (long wait times = bad UX)
❌ Quality drops (fake doctors, scams)
```

**Strategy to Capture Opportunity:**
```typescript
// Viral Growth Playbook
const viralPreparedness = {
  infrastructure: {
    action: 'Pre-provision auto-scaling to 100x capacity',
    cost: '€5k/month reserved instances (insurance)',
    trigger: 'Activate when signups >1000/day',
  },

  support: {
    action: 'AI chatbot + templated responses',
    implementation: 'Build in Month 3 (before launch)',
    fallback: 'Hire 5 support agents on-demand (Upwork)',
  },

  doctorRecruitment: {
    action: 'Waitlist for doctors with incentives',
    campaign: '€500 bonus for first 10 appointments',
    automation: 'Auto-approve verified doctors (PWZ license check)',
  },

  qualityControl: {
    action: 'Verification pipeline (PWZ number + SMS)',
    manual_review: 'First 3 appointments before full access',
    fraud_detection: 'Flag suspicious patterns (too cheap, fake reviews)',
  },
};
```

**Actionable Insights:**
> **Build viral infrastructure BEFORE virality**
> Pre-launch checklist: Auto-scaling ✅, Support chatbot ✅, Doctor waitlist ✅, Fraud detection ✅

---

#### **SCENARIO 2: What if EU mandates interoperability (FHIR) for all health apps?**

**Trigger:**
- EU Digital Health Regulation (2026)
- All apps MUST support FHIR data exchange
- Compliance deadline: 12 months

**Implications:**
```
Opportunities:
✅ YourMedic already has FHIR → Competitive advantage
✅ Competitors scramble (6-12 months to build)
✅ Clinics must integrate → We're ready, they're not
✅ Government grants for compliant platforms (€50-200k)

Challenges:
❌ Legacy clinics resist (old EHR systems)
❌ Data privacy concerns (patient hesitation)
❌ Certification costs (€30k for compliance audit)
```

**Strategy to Capture Opportunity:**
```
Month 0-3: Build FHIR MVP (already planned)
  ↓
Month 4-6: Apply for EU Digital Health Grant (€100k available)
  ↓
Month 7-9: Partner with 5 pilot clinics (government-funded)
  ↓
Month 10-12: Compliance certification (€30k investment)
  ↓
Month 13+: Marketing blitz "The only FHIR-compliant platform in PL"
  → Capture 40% market share while competitors build
```

**Actionable Insights:**
> **Regulatory compliance = moat**
> Invest €30k in FHIR certification early → 12-month head start on competitors

---

#### **SCENARIO 3: What if a major clinic chain (LuxMed, Medicover) wants to acquire YourMedic?**

**Trigger:**
- YourMedic hits 50,000 MAAC
- LuxMed sees us as threat (or opportunity)
- Acquisition offer: €10M

**Implications:**
```
Opportunities:
✅ Liquidity event (founders cash out)
✅ Distribution (LuxMed's 5M patients)
✅ Resources (their dev team, legal, compliance)
✅ Credibility (backed by industry leader)

Challenges:
❌ Loss of independence (strategic decisions)
❌ Product roadmap conflicts (their priorities vs yours)
❌ Culture clash (startup agility vs corporate bureaucracy)
❌ Potential shutdown (acqui-hire, kill competition)
```

**Decision Framework:**
```
Questions to ask:
1. Is this a strategic acquisition (they keep YourMedic alive)?
   → YES: Consider if price is right (3-5x revenue)
   → NO: Likely acqui-hire or kill → Reject

2. Do they commit to YourMedic independence?
   → Board seat + product autonomy = GREEN FLAG
   → Full integration = RED FLAG

3. What's our alternative path?
   → Can we raise Series A at similar valuation?
   → Is building solo more valuable long-term?

4. Financial needs:
   → €10M now vs €50M in 3 years (if we succeed)
   → Risk tolerance: Need money now? Accept.
   → Can sustain 3 years? Hold.
```

**Actionable Insights:**
> **Build for acquisition optionality, not necessity**
> Strong financials + growth = negotiating power. Don't sell out of desperation.

---

### **Category B: Challenging Scenarios**

---

#### **SCENARIO 4: What if Google/Apple launches a health booking platform?**

**Trigger:**
- Google Health integrates doctor booking into Search
- "dentysta Warszawa" → Book directly in Google Maps
- Zero friction, massive distribution

**Implications:**
```
Threats:
❌ Google has 90% search market share in PL
❌ Zero acquisition cost (already in search flow)
❌ Trust advantage (Google brand)
❌ Data advantage (search history = intent signals)

Opportunities:
✅ Google might partner (not build) → Be the backend
✅ Niche specialization (they're generic, we're medical-first)
✅ Quality differentiation (AI Symptom Checker, personalized care)
✅ Clinic relationships (we have contracts, they don't)
```

**Survival Strategy:**
```
Defense:
1. Lock in clinics with long-term contracts (12-24 months)
2. Build sticky features Google can't replicate:
   - Medical records storage (FHIR integration)
   - AI-powered follow-up (continuity of care)
   - Wearables integration (chronic disease management)

3. White-label for Google?
   - YourMedic = backend, Google = frontend
   - Revenue share model (30/70 split)
   - Scale to 10M users overnight

Offense:
1. Move upmarket (B2B Enterprise)
   - Sell to hospital chains (Google won't)
   - Custom integrations (EHR, billing)

2. Geographic expansion FAST
   - Launch in Czech, Slovakia, Hungary before Google
   - First-mover advantage in CEE
```

**Actionable Insights:**
> **Don't compete with giants on distribution - compete on depth**
> Build medical-specific moats: FHIR integration, AI diagnostics, chronic care management

---

#### **SCENARIO 5: What if AI becomes so good that patients self-diagnose accurately?**

**Trigger:**
- GPT-7 (2027) has 95% diagnostic accuracy
- Patients trust AI more than doctors
- "Why book appointment if AI can tell me?"

**Implications:**
```
Threats:
❌ Reduced appointment volume (AI replaces triage)
❌ Commoditization of basic consultations
❌ Doctor resistance (job threat)

Opportunities:
✅ AI handles triage → Doctors focus on complex cases
✅ YourMedic becomes AI provider (not just marketplace)
✅ Hybrid model: AI first, human second (cost-effective)
✅ New revenue stream: AI subscription (€9.99/month)
```

**Pivot Strategy:**
```
Evolution Path:

Phase 1 (Today): Doctor marketplace
  Revenue: 15% commission on appointments

Phase 2 (2026): AI + Doctor hybrid
  Revenue: €4.99/month AI subscription + commission
  Flow: Patient → AI triage → (if needed) Doctor referral

Phase 3 (2028): AI-first, human oversight
  Revenue: €19.99/month premium AI + telemedicine bundle
  Model: AI diagnosis → Doctor validates (2-min async review)

Phase 4 (2030+): AI healthcare OS
  Revenue: B2B2C (sell to insurers, employers)
  Product: Predictive health platform (AI + wearables + genetics)
```

**Actionable Insights:**
> **AI is not a threat - it's a force multiplier**
> Embrace AI to reduce costs, then layer human expertise for complex cases. Race to build best medical AI in Europe.

---

#### **SCENARIO 6: What if a data breach exposes 100,000 patient records?**

**Trigger:**
- Hacker exploits zero-day vulnerability
- Patient medical histories leaked to dark web
- GDPR complaint filed → €20M fine exposure

**Implications:**
```
Immediate:
❌ Platform shutdown (trust = 0)
❌ Media scandal (TVN, Onet, Gazeta)
❌ Legal liabilities (class action lawsuit)
❌ Clinic exodus (contract terminations)

Long-term:
❌ Brand damage (years to recover)
❌ Regulatory scrutiny (audits, restrictions)
❌ Insurance costs spike (cyber liability)
```

**Crisis Management Playbook:**
```
Hour 0-24: Containment
- Shut down affected systems
- Engage forensics team (€50k emergency)
- Notify GIODO (GDPR 72-hour requirement)
- Draft public statement (transparency)

Day 2-7: Notification
- Email all affected patients (legal requirement)
- Offer free credit monitoring (12 months, €100k cost)
- Hold press conference (CEO apology)
- Publish incident report (what happened, what we're doing)

Week 2-4: Remediation
- Patch vulnerability
- Third-party security audit (€30k)
- Implement recommendations
- Penetration testing (quarterly)

Month 2-6: Rebuild Trust
- ISO 27001 certification (€50k)
- Bug bounty program (€10k/year)
- Transparency reports (publish security metrics)
- Customer advisory board (patient advocates)

Total Crisis Cost: €250k + reputation damage
```

**Prevention Investment:**
```
Annual Security Budget: €75k
- Penetration testing (quarterly): €20k
- Security engineer (full-time): €40k
- Bug bounty program: €10k
- Cyber insurance: €5k

ROI: €75k/year prevention vs €250k+ crisis
```

**Actionable Insights:**
> **Security is not optional - it's existential**
> Budget €75k/year for security from Day 1. One breach = company death.

---

### **Category C: Market Disruption Scenarios**

---

#### **SCENARIO 7: What if COVID-like pandemic happens again?**

**Trigger:**
- New virus (2027)
- Lockdown 2.0
- In-person appointments banned for 6 months

**Implications:**
```
Opportunities:
✅ Telehealth demand 10x overnight
✅ Government contracts (official telemedicine platform)
✅ Investors pour money into healthtech
✅ Behavior change (patients comfortable with virtual care)

Challenges:
❌ Regulatory barriers (telemedicine laws unclear)
❌ Doctor resistance (older physicians not tech-savvy)
❌ Payment issues (NFZ doesn't reimburse telehealth)
❌ Infrastructure overload (10x traffic)
```

**Pandemic Playbook:**
```
Pre-pandemic (build optionality):
- Telehealth MVP (Month 6) ✅
- WebRTC video infrastructure ✅
- Doctor training program (telehealth best practices) ✅

Pandemic Day 1-7:
- Free telehealth for all users (PR + user acquisition)
- Partner with government (offer platform for €1)
- Media blitz ("YourMedic keeps Poland healthy")

Week 2-12:
- Scale infrastructure (10x capacity)
- Recruit 5,000 doctors (massive supply)
- Monetize: €10/consultation (insurance later)

Post-pandemic:
- Retain 30% of new users (habitual telehealth)
- Normalize hybrid care (in-person + virtual)
- Exit strategy: Acquisition by insurance company (€50M+)
```

**Actionable Insights:**
> **Build pandemic-proof features even in peacetime**
> Telehealth = 10% revenue today, 60% revenue in crisis. Optionality is valuable.

---

#### **SCENARIO 8: What if NFZ (Polish public insurance) mandates all bookings through one platform?**

**Trigger:**
- Government digitalization initiative
- NFZ selects ONE platform for all public health bookings
- Winner-takes-all tender (€100M contract)

**Implications:**
```
If YourMedic wins:
✅ Instant monopoly (38M citizens)
✅ €100M revenue guaranteed
✅ Scale = moat (no competitor can catch up)

If competitor wins:
❌ Locked out of 90% of market (public health)
❌ YourMedic = niche player (private only)
❌ Valuation drops 80%

If no platform wins (they build internally):
❌ Everyone loses (government platform usually bad)
❌ Opportunity: Sell to government as contractors
```

**Tender Winning Strategy:**
```
Pre-tender (6 months before):
1. Hire former NFZ executive (consultant, €50k)
   → Insider knowledge of tender criteria

2. Build government relationships
   → Present to Ministry of Health (demo platform)

3. Partnership with incumbent (Kamsoft, Mediporta)
   → Joint bid = higher chance (their relationships + our tech)

4. Compliance over-investment
   → ISO 27001, WCAG 2.1 (accessibility), Polish Cloud
   → Check every box in tender requirements

During tender:
5. Underbid slightly (€80M vs competitors' €100M)
   → Make up margin on future B2B products

6. Reference customers (10 major clinics)
   → Proof of scale & reliability

7. Highlight innovation (AI, telehealth)
   → Differentiate from legacy vendors

Win probability: 30% (long shot, but worth it)
ROI: €500k investment → €100M contract (200x)
```

**Actionable Insights:**
> **Play the long game with government**
> Even if you don't win tender, relationships = future partnerships. Never ignore public sector.

---

#### **SCENARIO 9: What if blockchain/Web3 enables patient-owned health records?**

**Trigger:**
- Patients demand data ownership (GDPR empowerment)
- Blockchain standard emerges (Health Chain Protocol)
- Patients control who sees their data → Monetize access

**Implications:**
```
Opportunities:
✅ New business model: Patients earn when sharing data
✅ Research revenue: Pharma pays patients for anonymized data
✅ Differentiation: "You own your data" (privacy brand)

Challenges:
❌ Technical complexity (blockchain integration)
❌ User experience nightmare (private keys, wallets)
❌ Regulatory uncertainty (is this legal?)
```

**Web3 Health Strategy:**
```
Phase 1 (Experiment): Patient data wallet (opt-in)
- Store health records on IPFS (decentralized)
- Patients control access via smart contracts
- €0.10 micropayment when pharma accesses anonymized data

Phase 2 (Scale): Health data marketplace
- Patients: Earn €50-200/year selling anonymized data
- Researchers: Buy datasets (€10k for 1,000 patient cohort)
- YourMedic: 20% platform fee (€2k commission)

Phase 3 (Ecosystem): Health token economy
- MEDIC token: Patients earn for healthy behaviors
- Redeem for: Free appointments, prescription discounts
- Clinics accept tokens (liquidity via YourMedic exchange)

Risks:
- Regulatory ban (GDPR might prohibit data sales)
- User adoption (too complex for mainstream)
- Token volatility (crypto winter kills momentum)

Go/No-Go Decision:
- Monitor regulatory signals (EU Web3 health stance)
- Pilot with 1,000 users (€50k budget)
- If >20% adoption → Scale. If <5% → Kill.
```

**Actionable Insights:**
> **Web3 = high risk, high reward**
> Don't bet company on it, but allocate 5% budget to experiment. Could be 10x differentiator or total flop.

---

### **Category D: Technology Breakthrough Scenarios**

---

#### **SCENARIO 10: What if wearables achieve medical-grade accuracy?**

**Trigger:**
- Apple Watch 10 (2028) gets FDA/EU MDR approval
- Continuous glucose, blood pressure, ECG = clinical accuracy
- Patients prefer wearables over doctor visits

**Implications:**
```
Opportunities:
✅ Passive health monitoring → Early disease detection
✅ Chronic disease management (diabetes, hypertension)
✅ New revenue: Wearables subscription (€9.99/month)
✅ Predictive health (AI + wearables = risk scores)

Challenges:
❌ Apple/Samsung capture value (not us)
❌ Doctors become "validators" (less revenue)
❌ Regulatory complexity (we become medical device)
```

**Wearables-First Strategy:**
```
Product Evolution:

Today: Wearables = nice-to-have
- Sync Fitbit, Apple Health (basic integration)
- Show stats in patient profile

2026: Wearables = diagnostic tool
- AI analyzes trends (heart rate variability, sleep)
- Alert: "Your BP trending up → Book cardiologist"
- Conversion: 15% of alerts → Appointments

2028: Wearables = primary care
- Continuous monitoring (chronic patients)
- Doctor reviews weekly (async)
- Revenue: €19.99/month subscription
- Model: 1 doctor manages 200 chronic patients

2030: Wearables = prevention engine
- Predictive health scores (0-100)
- Personalized interventions (diet, exercise, meds)
- B2B2C: Sell to employers (employee wellness)
- Revenue: €50/employee/year (100,000 employees = €5M ARR)
```

**Actionable Insights:**
> **Wearables are the future of primary care**
> Shift from reactive (wait for symptoms) to proactive (prevent disease). Build wearables integration in Month 6.

---

#### **SCENARIO 11: What if AI achieves AGI (Artificial General Intelligence)?**

**Trigger:**
- AGI emerges (2030+)
- AI can diagnose better than 99% of doctors
- Healthcare industry disrupted overnight

**Implications:**
```
Existential Questions:
- Do we need doctors anymore?
- What's YourMedic's role in AGI world?
- How do we adapt or die?

Opportunities:
✅ YourMedic = AGI interface (human-AI collaboration)
✅ Doctors become "AI supervisors" (validate edge cases)
✅ Healthcare becomes radically cheaper (€5 consultations)
✅ Global expansion (AGI speaks all languages)

Threats:
❌ Google/OpenAI dominate (we're too small)
❌ Regulation bans AGI doctors (protect human jobs)
❌ Society not ready (mass unemployment, resistance)
```

**AGI Adaptation Playbook:**
```
Scenario A: AGI is open-source (best case)
- Fine-tune AGI for Polish healthcare
- Integrate into YourMedic (free AI consultations)
- Differentiate: Local expertise + compliance

Scenario B: AGI is proprietary (OpenAI, Google)
- License AGI API (pay per query)
- Add value: YourMedic UX + patient relationships
- Risk: Margin compression (commodity)

Scenario C: AGI is regulated (EU bans autonomous diagnosis)
- Human-in-loop required by law
- YourMedic = compliant platform (AI + doctor validation)
- Competitive advantage: Only legal option

Hedge Strategy:
- Invest in AI talent NOW (build in-house capability)
- Partner with research labs (AGH University, Jagiellonian)
- Contribute to open-source medical AI (build influence)
```

**Actionable Insights:**
> **AGI is 5-10 years away, but prepare now**
> Hire AI researchers, build datasets, establish brand as "AI-first healthcare." When AGI arrives, you're ready.

---

**💎 KEY INSIGHTS: What If Scenarios**

**Offensive Opportunities:**
> 1. **Viral growth preparedness:** Pre-build auto-scaling, support chatbot, doctor waitlist BEFORE virality
> 2. **Regulatory moat:** Invest €30k in FHIR certification → 12-month head start on competitors
> 3. **Pandemic optionality:** Build telehealth even if demand is low → 10x revenue in crisis
> 4. **Wearables-first:** Shift to preventive care → €50/employee/year B2B2C model = €5M ARR
> 5. **AGI preparation:** Hire AI talent now → When AGI emerges, you're a player not a victim

**Defensive Strategies:**
> 1. **Google/Apple threat:** Compete on depth (FHIR, AI diagnostics, chronic care) not breadth (search)
> 2. **Acquisition preparedness:** Build for optionality → Strong financials = negotiating power
> 3. **Security investment:** €75k/year prevents €250k+ breach crisis → Non-negotiable
> 4. **Government relationships:** Play long game with NFZ → Even if tender fails, partnerships emerge
> 5. **Web3 experiment:** Allocate 5% budget to patient-owned data → Could be 10x differentiator

**Decision Rules:**
> - **Build pandemic-proof features even in peacetime** (telehealth, remote monitoring)
> - **Regulatory compliance = moat** (invest early when competitors ignore)
> - **Don't compete with giants on distribution - compete on depth** (medical expertise > scale)
> - **Security is existential** (one breach = company death)
> - **Embrace AI as force multiplier** (augment doctors, don't replace)

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
