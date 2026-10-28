# Računarstvo u oblaku

Materijali za predmet **Računarstvo u oblaku**. Prezentacije su javno dostupne u izvornom formatu (Quarto `.qmd`) i kao gotovi PDF fajlovi.

## Sadržaj

| #  | Tema                                     | Izvorni fajl                         | PDF                                                                   |
|----|------------------------------------------|--------------------------------------|-----------------------------------------------------------------------|
| 00 | Servisne informacije o predmetu          | [00.qmd](source/00.qmd)              | [PDF](PDFs/00-ServisneInformacije.pdf)                                |
| 01 | Uvod u računarstvo u oblaku              | [01.qmd](source/01.qmd)              | [PDF](PDFs/01-Uvod.pdf)                                               |
| 02 | Mrežne tehnologije računarstva u oblaku  | [02.qmd](source/02.qmd)              | [PDF](PDFs/02-MrezneTehnologijeRačunarstvaUOblaku.pdf)                |
| 03 | Virtualizacija i kontejnerizacija        | [03.qmd](source/03.qmd)              | [PDF](PDFs/03-VirtualizacijaKontejnerizacija.pdf)                     |

## Struktura repozitorijuma

```text
.
├── PDFs/      # gotove prezentacije u PDF formatu
└── source/    # izvorni .qmd fajlovi
    └── img/   # slike koje koriste prezentacije
```

## Generisanje prezentacija

### Potreban softver

- [Quarto](https://quarto.org/docs/get-started/) verzija **1.8** ili novija

Instalirana verzija se proverava komandom:

```bash
quarto --version
```

### Pokretanje

Komande se pokreću iz foldera `source/`, da bi putanje do slika bile ispravne:

```bash
cd source
quarto preview 00.qmd
```

Umesto `00.qmd` navedite fajl koji vam treba. Prezentacija se otvara u pregledaču i automatski osvežava pri svakoj izmeni fajla.

Za trajni HTML fajl, bez pokretanja servera:

```bash
quarto render 00.qmd
```
