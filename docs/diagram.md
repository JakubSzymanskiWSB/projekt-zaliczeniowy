# 📊 Schemat przepływu użytkownika

```mermaid
graph TD
    A[Start: Ekran Powitalny] --> B{Zalogowany?}
    B -- Nie --> C[Rejestracja]
    B -- Tak --> D[Panel Główny]
    C --> D
    D --> E[Wybierz Eko-Zadanie]
    D --> F[Zobacz Statystyki]
    E --> G[Zatwierdź wykonanie]
    G --> D
    F --> D