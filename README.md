
# Research-Pages
Surveys for research
flowchart TD
    A[Użytkownik wchodzi na stronę rekrutacyjną] --> B[Czyta opis badania i kryteria udziału]
    B --> C[Wybiera: Ból kolana lub Ból pięty]
    C --> D[Przekierowanie do formularza kwalifikacyjnego w REDCap]

    D --> E{Spełnia kryteria?}
    E -->|Nie| F[Komunikat: dziękujemy, brak kwalifikacji]
    E -->|Tak| G[Formularz zgłoszeniowy: dane dziecka, dane rodzica, zgoda RODO]

    G --> H{Ścieżka udziału}
    H -->|Kwestionariusze| I[Wypełnienie KOOS-Child + AKPS lub OxAFQ-C w REDCap]
    H -->|Rozmowa wideo| J[Wybór terminu rozmowy i link do spotkania]

    I --> K[Test–retest: automatyczne przypomnienie po 7–14 dniach]
    K --> L[Drugie wypełnienie kwestionariuszy]
    J --> L
    L --> M[Zakończenie udziału, eksport danych do analizy]
