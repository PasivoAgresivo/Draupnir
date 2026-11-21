# Draupnir

Rodinná webová aplikace na zapisování jídla a kalorií (později i tréninků).
Běží na GitHub Pages, data jsou v Supabase.

- **Jídelníček:** zápis jídel po dnech (snídaně, svačiny, oběd, večeře), součty kalorií a maker proti dennímu cíli.
- **Potraviny:** společná databáze potravin pro celou rodinu, hodnoty na 100 g. Skenování čárových kódů a dohledání přes [Open Food Facts](https://openfoodfacts.org) (data pod licencí ODbL).
- **Profil:** denní cíl zadaný ručně nebo dopočítaný (Mifflin–St Jeor), zápis váhy, změna hesla.

Každý uživatel vidí jen svůj jídelníček a váhu, hlídá to Row Level Security v databázi.
Účty zakládá správce v Supabase (veřejná registrace je vypnutá).
V kódu je jen veřejný (publishable) klíč, který je určený k tomu, aby byl vidět.
