# Homework_helper
# Domácí spotřebiče / Household Appliances

-   [Česky](#česky)
-   [English](#english)

------------------------------------------------------------------------

# Česky

## Popis

Samostatná webová aplikace v jednom souboru HTML. Aktuální verze
obsahuje interaktivní tabulku pro kontaktní gril a připravenou položku
pro pračku.

Aplikace je navržena především pro použití na mobilním telefonu.

## Funkce

### Kontaktní gril

-   Výběr funkce: Chléb, Steak, Kuře, Ryba, Párek, Slanina nebo
    Hamburger.
-   Zadání tloušťky v milimetrech.
-   Výběr stupně propečení.
-   Automatická aktualizace doporučené teploty a doby podle zvolených
    hodnot.
-   Zobrazení celé tabulky pro zvolenou funkci pod výsledkem.
-   Zvýraznění použitého řádku a sloupce odpovídajícího stupni
    propečení.
-   Zobrazení dostupných rozsahů tloušťky.
-   Upozornění, pokud pro zadanou tloušťku neexistuje přesný záznam v
    tabulce.

### Pračka

Sekce pračky je zatím pouze informační a neobsahuje ovládací funkce.

## Použití

1.  Otevřete soubor `domaci_spotrebice_merged.html` v moderním webovém
    prohlížeči.
2.  Na úvodní obrazovce zvolte **Grill**.
3.  Vyberte funkci grilu.
4.  Zadejte tloušťku v milimetrech.
5.  Zvolte stupeň propečení.
6.  Výsledek se aktualizuje automaticky. Níže se zobrazí celá tabulka
    pro zvolenou funkci.
7.  Tlačítkem **Spotřebiče** se vrátíte na úvodní obrazovku.

Aplikace pracuje s celými čísly. Pokud zadáte desetinnou hodnotu,
převede ji na nejbližší celé číslo pomocí JavaScriptové funkce
`Math.round()`.

## Rozsahy tloušťky

Rozsahy jsou převzaty z dodané tabulky. Rozsah **25--30 mm** nahrazuje
původní rozsah **26--30 mm** u funkcí, kde byl tento řádek uveden.
Hodnoty doby a teploty v tomto řádku zůstaly převzaté z původního
záznamu; nejde o samostatně ověřené doporučení pro každý jednotlivý
milimetr v rozsahu.

Pokud zadaná tloušťka nemá v tabulce přesný záznam, aplikace může použít
nejbližší dostupný řádek a zobrazí upozornění.

## Spuštění a požadavky

-   Není potřeba instalace.
-   Není potřeba server ani databáze.
-   Hlavní logika a data jsou uloženy přímo v HTML souboru.
-   Aplikaci lze otevřít lokálně v prohlížeči.
-   Externí písmo Barlow se načítá z Google Fonts. Bez internetového
    připojení se použije dostupné systémové písmo; hlavní funkce
    aplikace zůstávají lokální.

## Omezení a upozornění

-   Údaje o teplotě a době jsou převzaty z dodané tabulky. Aplikace je
    nezávisle neověřuje.
-   Zobrazená doba sama o sobě nezaručuje bezpečnou tepelnou úpravu
    potravin. Výsledek závisí mimo jiné na konkrétním grilu, počáteční
    teplotě a vlastnostech potraviny.
-   U kuřecího masa dbejte na dostatečnou tepelnou úpravu; neřiďte se
    pouze zobrazeným časem.
-   Data jsou součástí HTML souboru. Při změně zdrojové tabulky je nutné
    aktualizovat data v aplikaci.
-   Sekce pračky není implementována.

## Soubory

-   `domaci_spotrebice_merged.html` --- vlastní aplikace.
-   `README.md` --- tento návod.

## Technické informace

Aplikace používá HTML, CSS a JavaScript bez potřeby serverové části.
Uživatelské rozhraní reaguje na změnu výběru a zadané tloušťky bez
nutnosti odesílat data na server.

------------------------------------------------------------------------

# English

## Description

A standalone web application contained in a single HTML file. The
current version includes an interactive contact-grill table and a
placeholder section for a washing machine.

The application is primarily designed for use on mobile phones.

## Features

### Contact grill

-   Select a food/function: Bread, Steak, Chicken, Fish, Sausage, Bacon,
    or Hamburger.
-   Enter the thickness in millimetres.
-   Select the desired doneness level.
-   Automatically update the suggested temperature and cooking time
    based on the selected values.
-   Display the complete table for the selected function below the
    result.
-   Highlight the matching row and the column for the selected doneness
    level.
-   Display the available thickness ranges.
-   Show a warning when the table does not contain an exact record for
    the entered thickness.

### Washing machine

The washing-machine section is currently informational only and does not
provide operating controls.

## How to use

1.  Open `domaci_spotrebice_merged.html` in a modern web browser.
2.  Select **Grill** on the home screen.
3.  Choose the grill function.
4.  Enter the thickness in millimetres.
5.  Select the desired doneness level.
6.  The result updates automatically. The complete table for the
    selected function appears below it.
7.  Use the **Appliances** button to return to the home screen.

The application works with whole numbers. If you enter a decimal value,
it is rounded to the nearest integer using JavaScript's `Math.round()`
function.

## Thickness ranges

The ranges are based on the supplied table. For functions where the
original **26--30 mm** row was present, it has been changed to **25--30
mm**. The cooking-time and temperature values remain those from the
original row; they have not been independently verified for every
individual thickness in the range.

If the entered thickness has no exact match in the table, the
application may use the nearest available row and display a warning.

## Launching and requirements

-   No installation is required.
-   No server or database is required.
-   The main logic and data are embedded in the HTML file.
-   The application can be opened locally in a web browser.
-   The Barlow font is loaded from Google Fonts. Without an internet
    connection, the browser uses an available system font; the
    application's main functionality remains local.

## Limitations and safety notes

-   Temperature and cooking-time values are taken from the supplied
    table and have not been independently verified by the application.
-   The displayed time alone does not guarantee that food has been
    cooked safely. The result also depends on the grill, the food's
    starting temperature, and other characteristics.
-   Ensure chicken is cooked thoroughly; do not rely on the displayed
    time alone.
-   The data is embedded in the HTML file. When the source table
    changes, the application's embedded data must also be updated.
-   The washing-machine section has not been implemented.

## Files

-   `domaci_spotrebice_merged.html` --- the application.
-   `README.md` --- this documentation.

## Technical details

The application uses HTML, CSS, and JavaScript and does not require a
server-side component. The interface reacts to changes in the selected
options and entered thickness without sending data to a server.
