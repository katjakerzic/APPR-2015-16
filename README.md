# Analiza podatkov s programom R, 2015/16

Avtor: Katja Keržič
#
Repozitorij z gradivi pri predmetu APPR v študijskem letu 2015/16.

## Tematika

Naslov mojega projekta je: Analiza svetovnih cen žit. V projektu bom analizirala spremembe cen žit v letih od 2009 do 2013. Projekt bo v tabeli vseboval države sveta in različne vrste žit (pšenica, ječmen, rž...).

Moj cilj je ugotoviti, kako so se gibale svetovne cene žit (2009-2013), potem pa primerjati te podatke s spremembami cen po posameznih kontinentih v istem obdobju. 

Podatke za projekt sem dobila na spletni strani Organizacije Združenih narodov za prehrano in kmetijstvo: http://faostat3.fao.org/download/P/PP/E


## Program

Glavni program in poročilo se nahajata v datoteki `projekt.Rmd`. Ko ga prevedemo,
se izvedejo programi, ki ustrezajo drugi, tretji in četrti fazi projekta:

* obdelava, uvoz in čiščenje podatkov: `uvoz/uvoz.r`
* analiza in vizualizacija podatkov: `vizualizacija/vizualizacija.r`
* napredna analiza podatkov: `analiza/analiza.r`

Vnaprej pripravljene funkcije se nahajajo v datotekah v mapi `lib/`. Podatkovni
viri so v mapi `podatki/`. Zemljevidi v obliki SHP, ki jih program pobere, se
shranijo v mapo `../zemljevidi/` (torej izven mape projekta).

## Spletni vmesnik

Spletni vmesnik se nahaja v datotekah v mapi `shiny/`. Poženemo ga tako, da v
RStudiu odpremo datoteko `server.R` ali `ui.R` ter kliknemo na gumb *Run App*.
Alternativno ga lahko poženemo tudi tako, da poženemo program `shiny.r`.

## Potrebni paketi za R

Za zagon tega vzorca je potrebno namestiti sledeče pakete za R:

* `knitr` - za izdelovanje poročila
* `rmarkdown` - za prevajanje poročila v obliki RMarkdown
* `shiny` - za prikaz spletnega vmesnika
* `DT` - za prikaz interaktivne tabele
* `maptools` - za uvoz zemljevidov
* `sp` - za delo z zemljevidi
* `digest` - za zgoščevalne funkcije (uporabljajo se za shranjevanje zemljevidov)
* `httr` - za pobiranje spletnih strani
* `XML` - za branje spletnih strani
* `extrafont` - za pravilen prikaz šumnikov (neobvezno)
