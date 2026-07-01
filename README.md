# Wycinka drzew Rzeszów — landing page

Jednostronicowa, samodzielna strona (one-pager) dla firmy świadczącej
alpinistyczną (sekcyjną) wycinkę i pielęgnację drzew w Rzeszowie i okolicach.

- **Jeden plik:** `index.html` — cały HTML, CSS i JS w środku. Bez frameworków
  i bibliotek. Można hostować gdziekolwiek (Netlify, GitHub Pages, zwykły serwer).
- **Mobile-first**, responsywny do 360 px, dostępność (kontrast AA, widoczny
  focus klawiatury, aria-label), dane strukturalne schema.org (LocalBusiness).
- **Sygnatura wizualna:** pionowa „lina asekuracyjna”, która dorysowuje się przy
  przewijaniu (wyłączana przy `prefers-reduced-motion`).

## ✅ Co uzupełnić przed publikacją

Wszystkie miejsca do zmiany są oznaczone w kodzie `index.html` w nawiasach
`[...]` oraz komentarzami `<!-- ZMIEŃ ... -->`. Najważniejsze:

| Placeholder            | Gdzie                                    |
|------------------------|------------------------------------------|
| `[NAZWA FIRMY]`        | pasek górny, hero, stopka, schema.org    |
| `[NR TELEFONU]`        | tekst przycisków + `href="tel:+48..."`   |
| `[E-MAIL]`             | kontakt + stopka + `href="mailto:..."`   |
| `[NIP]`                | stopka + `vatID` w schema.org            |
| `[TWOJA-DOMENA].pl`    | canonical, Open Graph, schema.org        |
| Zdjęcia                | `<!-- === WSTAW ZDJĘCIE ... === -->`     |
| Opinie                 | sekcja „Opinie” — podmień na realne z Google |
| Linki social / Google  | stopka i sekcja opinii                   |

> **Telefon:** zmień numer w **dwóch miejscach** każdego linku — w widocznym
> tekście oraz w atrybucie `href="tel:+48XXXXXXXXX"` (bez spacji, z `+48`).

## 📷 Zdjęcia

Zdjęcia są na razie eleganckimi placeholderami. Podmień je na realne fotografie
pracy w koronie (liny, sprzęt) oraz efekty „przed/po”. Miejsca wstawienia
opisano w komentarzach. Dla hero podmień tło w regule `.hero__bg`.

## 📨 Formularz kontaktowy

Formularz jest gotowy pod **Formspree** lub **Netlify Forms** — wybierz jeden
wariant (instrukcja w komentarzu nad `<form>` w `index.html`):

- **Formspree:** ustaw `action="https://formspree.io/f/TWÓJ_ID"`, usuń atrybuty
  Netlify (`data-netlify`, `netlify-honeypot`) oraz ukryte pole `form-name`.
- **Netlify Forms:** zostaw `data-netlify="true"` i ukryte pole `form-name`;
  załączniki działają dzięki `enctype="multipart/form-data"`.

## 🚀 Publikacja

To zwykły plik statyczny — wgraj `index.html` na dowolny hosting albo przeciągnij
folder do Netlify. Nie ma kroku budowania (`build`).
