# it_toolkit

Sbírka IT skriptů a nástrojů pro správu a údržbu systémů.

## Struktura repozitáře

```
it_toolkit/
├── scripts/
│   ├── windows/
│   │   ├── batch/        # .bat / .cmd skripty
│   │   └── powershell/   # .ps1 skripty
│   └── linux/            # .sh skripty
└── docs/                 # doplňková dokumentace
```

## Obsah

| Skript | Platforma | Popis |
| ------ | --------- | ----- |
| _(zatím prázdné)_ | | |

## Použití

1. Naklonuj repozitář:
   ```bash
   git clone https://github.com/ggai/it_toolkit.git
   ```
2. Vyber skript v příslušné podsložce a přečti si jeho hlavičku (popis, požadavky, parametry).
3. Skript spusť podle platformy:
   - Windows batch: dvojklik nebo `cmd /c script.bat`
   - Windows PowerShell: `powershell -ExecutionPolicy Bypass -File script.ps1`
   - Linux: `chmod +x script.sh && ./script.sh`

## Konvence

- Každý skript má na začátku komentářovou hlavičku: název, popis, autor, datum, požadovaná oprávnění, parametry.
- Názvy souborů: malá písmena, slova oddělená podtržítkem (např. `clean_temp_files.bat`).
- Destruktivní operace (mazání, úpravy registru) musí mít potvrzovací dotaz nebo přepínač pro suchý běh.
- Skripty logují svou činnost, ať je dohledatelné, co se stalo.

## Upozornění

Skripty mohou zasahovat do systému a mazat data. Před spuštěním v produkci je vždy otestuj v testovacím prostředí. Použití je na vlastní riziko.

## Licence

Viz [LICENSE](LICENSE).
