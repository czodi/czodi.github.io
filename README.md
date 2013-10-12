# DataLeaks

Otevřená data přináší prospěch všem. Proto vidíme jako nesmyslné, když státní aparát, přes všechna svá prohlášení a výroky nabízí svým občanům naprosto zanedbatelné množství dat, často navíc v nepoužitelných, proprietárních či jinak nevhodných formátech. Naším cílem není změnit situaci pomocí nějakého zázraku přes noc. Spíš nám jde o to přispět svou troškou do mlýna a nabídnout některá data prostřednictvím otevřených formátů těm, kteří o ně budou stát. Rozhodně je naše snaha během na velice dlouhé trati, která možná ani nemá cíl. Přesto věříme, že někteří lidé naši činnost ocení a třeba se i odhodlají přispět k naší snaze svým volným časem a pomůžou nám tak dosáhnout lepších a kvalitnějších výsledků.

## Co je naším cílem
1. nabídnout data ve formátech, které **usnadní další použití** těchto dat
2. nabídnout veškerá data v **kódování UTF-8**
3. nabídnout snadným způsobem **verzovaná data** těm, kteří o to budou stát

## Formáty
Pro uložení dat jsme se rozhodli použít především **textové formáty**, které umožní snadné verzování pomocí verzovacího systému, hlavně ale zjednodušší vizualizaci změn mezi vybranými verzemi dat (diff). Prozatím máme vybrán formát pro uložení tabulkových dat, formáty pro uložení jiných typů dat budou vybrány ve chvíli, kdy bude nutné taková data zpracovat a uložit. Výběr takového formátu nyní by bylo podle nás zbytečně vynaložené úsilí.

### CSV - formát pro tabulková data
* obsah souboru bude uložen v kódování **UTF-8**
* pro oddělení jednotlivých sloupců bude použit znak čárky (`,`)
* textové hodnoty, případně hodnoty obsahující čárku, budou uzavřeny do uvozovek (`"`)
* pokud má hodnota obsahovat uvozovky, budou tyto zdvojeny (`Felicia "Fun"` → `Felicia ""Fun""`)
* datum a čas: viz sekce **Datum a čas**
* u desetinných čísel bude celá a desetinná část oddělena tečkou (`3.14`)
* jako oddělovač řádků bude použit pouze znak "\n" (`LF` - ASCII kód **10** (`0a`))

### Datum a čas
* datum a čas bude uložen ve formátu `YYYY-MM-DDTHH:MM:SS`
* datum: `YYYY-MM-DD`
* měsíc konkrétního roku: `YYYY-MM`
* čas: `HH:MM:SS`
* čas - pouze hodiny a minuty: `HH:MM`

(c) Czech OpenData Initiative
