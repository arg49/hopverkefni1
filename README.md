
# Hópverkefni 1

## Hvernig keyra á verkefnið

* Fyrst skal gera nýtt local repository með því að búa til nýja möppu, opna git í þeirri möppu og skrifa inn skipunina "git init"

* Næst skal skrifa "git clone" og vísa í eftirfarandi slóð: 
    
    ```bash
    https://github.com/arg49/hopverkefni1

Það virkar líka að gera þetta fyrst án þess að hafa gert "git init".

* Svo þarf að setja upp nodejs (ef það er ekki nú þegar sett inn) af þessari slóð: https://nodejs.org/en/, annað hvort nýjustu útgáfu eða útgáfu 8.12.0.

* Við mælum með að bæta við stylelint extension í Visual studio code.

* Til að keyra forritin í möppunni skal slá inn eftirfarandi skipanir:

    ```bash
    npm install -g sass
    npm install -g browser-sync
    npm install
    npm run dev

* Ef það virkar ekki að keyra dev eða ef sass og/eða browser-sync fara ekki sjálfkrafa af stað skal prófa að keyra sass og/eða browser-sync sérstaklega með eftirfarandi skipunum:

    ```bash
    npm run sass
    npm run browser-sync

Svo skal reyna run dev aftur.

* Til að keyra stylelint:

    ```bash
    npm run lint

* Til að uppfæra repository og setja þínar breytingar inná git:

    ```bash
    git status
    git pull
    git commit -a
    -> þú færð upp nýjan valglugga og þarft að gera eftirfarandi:
       i
       skifa inn hverju var breytt 
       ýta á esc
       :wq
    git push origin <branch> <- Við unnum bara með branch = master

## Lýsing

* Verkefnið er allt geymt inni í möppu sem ber heitið "hopverkefni1" og inni í henni eru eftirfarandi skrár:
     ```bash
     Aðal:
     index.html
     grid.css
     README.md
     styles.scss
     styles.css

     Auka:
     .editorconfig
     .gitattributes
     .gitignore
     .stylelintrc
     package.json
     package-lock.json

     Möppur:
     img
     pages
     scss
     utlit
     node_modules

* Inni í möppunni "pages" má finna html fyrir allar síður nema forsíðu
    ```bash
    products.html er síðan með sýnir vöruúrval Vöruhússins.
    staff.html er fyrir síðuna með upplýsingum um starfsfólk.
    cart.html er fyrir síðuna með innkaupakörfunni.

* Í img möppu má finna myndirnar sem eru á síðunni, í utlit möppu er fyrirmynd að útliti á síðunum og í efni má finna allan texta sem notaður er á síðunum.

* CSS skjalið er skipulagt þannig að efst eru grunn skipanir sem eiga við öll html skjölin, svo eru skipanir fyrir haus efst, svo forsíðu, næst starfsmannasíðu, svo vörusíðu, næst körfusíðu og að lokum kemur fóturinn neðst.

* Við unnum verkefnið þannig að Arnþór sá um haus, starfsmannasíðu, körfusíðu og kláraði vörusíðu (vegna fjarveru Kristófers), Jóhann sá um fót, forsíðu og körfusíðu, Kristófer sá um vörusíðu og svo hjálpuðust allir að fyrir tilfallandi vandamál.

* Í öllum html skjölunum má finna sama haus og fót en svo skrifaði hver og einn html fyrir þá síðu sem hann var að vinna að.

* Þetta README skjal er skrifað af Arnþóri og Jóhanni.

## Allir sem unnu að verkefninu

* Arnþór Guðmundsson           - arg49
* Jóhann Sigurður Jóhannsson   - JohannSJohannsson
* Kristófer Darri Finnsson     - KristoferDarri


# Verkefnislýsing frá kennara að hópverkefni 1

Verkefnið felst í því að smíða vef eftir forskrift.

Gefnar eru [fyrirmyndir](utlit/) í `500px`, `800px` og `1500px` með grind ásamt `1500px` án grindar og yfirliti yfir virkni vefs í `utlit/video.mp4`.

## Síður

Gögn fyrir síður eru í viðeigandi textaskrám (t.d. forsida.txt) undir `efni/`. Myndir fyrir síður eru gefnar undir `img/`. Afrita þarf öll gögn á milli síðna, ekki er krafa um að setja upp sameiginlegan haus/fót á síðum með einhverju kerfi eða forritun.

Efni síðu skal ekki vera breiðara en `1200px`. Litir í haus og fæti skulu fylla út í allt lárétt pláss.

Síður hafa allar sama haus og sama fót. Vöruflokkar í fæti skulu allir vísa á `pages/products.html`.

Grunn leturstærð er 16px og fylgja allar aðrar leturgerðir eftirfarandi skala: `12 14 16 18 21 24 36 48 60`.

Litapalletta fyrir vef er `#000000`, `#ffffff`, `#afb281`, `#cee8ff`, `#fcffd2` og `#cc9694`.

Letur fyrir meginmál er Open Sans eða helvetica, arial eða sans-serif letur.
Letur fyrir fyrirsagnir er Oswald, Verdana eða serif letur.

Flest allt er sett upp í 12 dálka grind með `20px` gutter.

Öll bil eru hálft, heilt, tvöfalt eða þrefalt margfeldi af gutter. Hægt er að nota reglustiku tól (t.d. http://www.arulerforwindows.com/ eða http://www.pascal.com/software/freeruler/) til að finna nákvæmar stærðir en mestu skiptir að lausn svipi til en sé ekki nákvæmlega eins og fyrirmynd.

Allar hreyfingar gerast á `300ms` með `ease-in-out` hröðunarfalli.

Ekki þarf að útfæra neina virkni fyrir takka eða form.

## Hópavinna

Verkefnið skal unnið í hóp með þremur einstaklingum. Hafið samband við kennara ef ekki er mögulegt að vinna í hóp.

Notast skal við Git og GitHub. Engar zip skrár með kóða ættu að ganga á milli í hópavinnu, heldur á að „committa“ allan kóða og vinna gegnum Git.

## Lýsing á verkefni

`README.md` skrá skal vera í rót verkefnis og innihalda:

* Upplýsingar um hvernig keyra skuli verkefnið
* Lýsingu á uppsetningu verkefnis, hvernig því er skipt í möppur, hvernig CSS er skipulagt og fleira sem á við
* Upplýsingar um alla sem unnu verkefni
* Leyfilegt er að halda eftir þessari verkefnalýsingu en hún skal þá koma _á eftir_ ykkar lýsingu

## Tæki og tól

Setja skal upp Sass og stylelint fyrir verkefnið. Gefin er `styles.scss` skrá með grunn upplýsingum.

Gefin er `.stylelintrc` skrá sem segir til um hvernig lint fyrir `scss` skrár skuli háttað.

Í `.gitignore` er `styles.css` hunsað sem þýðir að það verður _ekki_ checkað inn. Það er gert vegna þess að það er búið til af sass út frá `styles.scss`

## Gefnar skrár

Eftirfarandi er sett upp í verkefni:

* `.stylelintrc` með upplýsingum um hvernig stylelint eigi að haga sér. Setja þarf upp `stylelint-config-primer` pakkann
* `.gitignore` sem hunsar algengar skrár, [sjá nánar](https://help.github.com/ignore-files/)
* `.gitattributes` sem kemur í veg fyrir ósamræmi sem geta komið upp þegar unnið er á milli stýrikerfa
* `.editorconfig` sem samræmir notkun á tabs og spaces, bilum [og fleira](https://editorconfig.org/)
* `index.html` með vísun í `styles.css` og `grid.css` ásamt tómum skrám fyrir `products.html`, `about.html` og `cart.html` undir `pages/`, halda skal þessu skipulagi
* `grid.css` til að sjá grid sem fyrirmynd er unnin eftir

Setja þarf upp `package.json` og sækja viðeigandi pakka til að tæki og tól sem verkefnið á að nýta virki.

## Mat

* 10% - `README` eftir forskrift, tæki og tól uppsett
* 20% – Snyrtilegt, gilt (skv. stylelint) CSS/Sass, gilt og aðgengilegt HTML
* 30% – Almennt útlit
* 10% – Forsíða
* 10% – Vörulista síða
* 10% – Um síða
* 10% – Kaupa síða

## Sett fyrir

Verkefni sett fyrir í fyrirlestri mánudaginn 8. október 2018.

## Skil

Einn aðili úr hóp skal skila fyrir hönd allra og skila skal undir „Verkefni og hlutaprófa“ á Uglu í seinasta lagi fyrir lok dags föstudaginn 26. október 2018.

Skil skulu innihalda:

* Nöfn allra í hóp ásamt notendanafni
* Slóð á GitHub repo fyrir verkefni, og dæmatímakennurum skal hafa verið boðið í repo ([sjá leiðbeiningar](https://help.github.com/articles/inviting-collaborators-to-a-personal-repository/)). Notendanöfn þeirra eru `arnar44`, `gorri4`, `mimiqkz`, `hinriksnaer`, `gunkol`, `freyrdanielsson` og `osk`
* Slóð á verkefnið keyrandi á vefnum

## Einkunn

Sett verða fyrir tíu minni verkefni þar sem átta bestu gilda 3,5% hvert, samtals 28% af lokaeinkunn.

Sett verða fyrir tvö stærri verkefni þar sem hvort um sig gildir 11%, samtals 22% af lokaeinkunn.

## Myndir

Myndir frá:

* [Innkaupakörfu íkon eftir Stephen Hutchings á www.flaticon.com](https://www.flaticon.com/authors/stephen-hutchings)
* Unsplash
  - https://unsplash.com/photos/MohB4LCIPyM
  - https://unsplash.com/photos/tpLz5aKdQmM
  - https://unsplash.com/photos/_T4w3JDm6ug
  - https://unsplash.com/photos/cOJgO4Zzs-w
  - https://unsplash.com/photos/PDX_a_82obo
  - https://unsplash.com/photos/ArGvQkA7iOw
  - https://unsplash.com/photos/5ExRBlHu1DA
  - https://unsplash.com/photos/b9dS7hpi67w
  - https://unsplash.com/photos/asBwpysXVB4
  - https://unsplash.com/photos/-s6XYBp1WTc
  - https://unsplash.com/photos/wKOKidNT14w

---

> Útgáfa 0.1
