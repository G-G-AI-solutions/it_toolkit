# Šablona hlavičky skriptu

Každý nový skript začíná hlavičkou v komentáři. Níže jsou šablony pro jednotlivé platformy.

## Windows batch (.bat / .cmd)

```bat
@echo off
REM ============================================================
REM Nazev:       clean_temp_files.bat
REM Popis:       Co skript dela, jednou az dvema vetami.
REM Autor:       Jmeno
REM Vytvoreno:   2026-08-18
REM Opravneni:   Vyzaduje spusteni jako Administrator (ano/ne)
REM Parametry:   /dry-run  vypise akce bez skutecneho mazani
REM              /quiet    potlaci potvrzovaci dotazy
REM Poznamky:    Znama omezeni, testovano na Windows 10/11.
REM ============================================================
```

Poznámka: v batch skriptech se vyhýbej diakritice, konzole ji standardně nezobrazuje správně.

## PowerShell (.ps1)

```powershell
<#
.SYNOPSIS
    Krátký popis skriptu.
.DESCRIPTION
    Podrobnější popis toho, co skript dělá.
.PARAMETER DryRun
    Vypíše akce bez provedení změn.
.EXAMPLE
    .\clean_temp_files.ps1 -DryRun
.NOTES
    Autor: Jméno
    Vytvořeno: 2026-08-18
    Oprávnění: vyžaduje Administrator
#>
```

## Bash (.sh)

```bash
#!/usr/bin/env bash
# ============================================================
# Název:      clean_temp_files.sh
# Popis:      Co skript dělá.
# Autor:      Jméno
# Vytvořeno:  2026-08-18
# Oprávnění:  vyžaduje root (ano/ne)
# Parametry:  --dry-run, --quiet
# ============================================================
set -euo pipefail
```
