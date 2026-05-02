# Pomarańczowa Plaża — menu online z panelem CMS

To jest gotowa paczka strony menu online. Strona działa od razu, a zdjęcia dań można dodawać później z panelu `/admin/`.

## Co jest w paczce

- `index.html` — strona menu dla gości.
- `data/menu.json` — baza pozycji menu: nazwy, ceny, opisy, zdjęcia.
- `admin/` — panel CMS do edycji menu i dodawania zdjęć.
- `images/uploads/` — tutaj CMS będzie zapisywał zdjęcia.
- `netlify.toml` — ustawienie dla Netlify.

## Ważne

Panel CMS działa najlepiej, gdy strona jest podłączona do repozytorium GitHub lub GitLab. Samo ręczne przeciągnięcie folderu do Netlify opublikuje stronę, ale panel CMS nie będzie mógł zapisywać zmian.

## Najprostszy sposób uruchomienia z CMS

1. Załóż konto na GitHub.com, jeśli go nie masz.
2. Utwórz nowe repozytorium, np. `pomaranczowa-plaza-menu`.
3. Wgraj wszystkie pliki z tej paczki do repozytorium.
4. W Netlify wybierz: Add new project → Import an existing project.
5. Połącz Netlify z GitHubem i wybierz to repozytorium.
6. Build command zostaw puste.
7. Publish directory ustaw jako `.` albo zostaw puste, jeśli Netlify wykryje `netlify.toml`.
8. Opublikuj stronę.
9. W Netlify włącz Identity oraz Git Gateway.
10. Wejdź na `https://twoja-strona.netlify.app/admin/` i zaloguj się zaproszonym adresem e-mail.

## Jak dodawać zdjęcia

1. Wejdź na `/admin/`.
2. Otwórz „Menu restauracji” → „Pozycje menu”.
3. Znajdź danie, np. „Łosoś pieczony w ziołach”.
4. W polu „Zdjęcie” dodaj fotografię.
5. Kliknij Save / Publish.
6. Netlify automatycznie przebuduje stronę, a QR zostaje ten sam.

## Jak działa brak zdjęcia

Jeśli pole „Zdjęcie” jest puste, strona pokaże grafikę zastępczą i napis „Zdjęcie wkrótce”.

## Jak zmienić ceny lub opisy

W panelu `/admin/` edytujesz nazwę, cenę, opis, kategorię i zdjęcie. Po zapisaniu zmiany pojawią się na stronie po krótkiej chwili.
