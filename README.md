# SharkOS — wydania

Oficjalne wydania systemu **SharkOS** (na bazie Debiana 13 „trixie”).

## Obrazy instalacyjne
Pobierz z zakładki **[Releases](https://github.com/halk6000/sharkos-wydania/releases)**:

| Plik | Do czego |
|---|---|
| `sharkos-<wersja>-mini-amd64.iso` (ok. 90 MB) | mały instalator: system pobiera się z internetu w trakcie instalacji (kabel albo Wi-Fi Intel) |
| `sharkos-<wersja>-amd64.iso` (ok. 800 MB) | pełny instalator Debiana z SharkOS |
| `*.sha256` | suma kontrolna — sprawdź przed zapisem na pendrive |

Zapis na pendrive: Rufus w trybie **„obraz DD”** albo `dd`. Instalator „obok innych systemów” działa tylko w trybie UEFI.

## Repozytorium pakietów (aktualizacje)
Zainstalowany SharkOS pobiera aktualizacje pakietu `sharkos` przez `apt` z
`https://halk6000.github.io/sharkos-wydania/` (gałąź `gh-pages` tego repozytorium).
Repozytorium jest podpisane kluczem OpenPGP o odcisku:

```
EA96 944A 47ED DFD1 ADF5  CD59 485B 8170 7D3F DADA
```

Klucz publiczny: [`sharkos-archive-keyring.asc`](https://halk6000.github.io/sharkos-wydania/sharkos-archive-keyring.asc)
(jest też w pakiecie `sharkos` jako `/usr/share/keyrings/sharkos-archive-keyring.gpg`).

## Licencje i kod źródłowy
Obrazy zawierają oprogramowanie Debiana na licencjach wolnego oprogramowania (m.in. GNU GPL).
Kod źródłowy tych pakietów jest dostępny w archiwum Debiana: https://sources.debian.org/ oraz
`deb-src http://deb.debian.org/debian trixie main non-free-firmware` (wersje zgodne z wydaniem w opisie Releases).
Na życzenie udostępnimy źródła odpowiadające konkretnemu obrazowi — napisz w zakładce Issues.

Pakiet `sharkos` (nakładka, usługi, narzędzia SharkOS) © halk6000. Wszelkie prawa zastrzeżone, o ile nie zaznaczono inaczej.
