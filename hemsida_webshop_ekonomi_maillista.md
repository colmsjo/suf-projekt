## Change log

| Datum  | Namn          |  Uppdatering                                             |
|--------|---------------|----------------------------------------------------------|
| 180901 | Jonas Colmsjö |  Första version |
| 181011 | Jonas Colmsjö |  Bytt namn på filen och lagt till hemsida och maillistor |
| 181023 | Jonas Colmsjö |  Uppdaterat med info om Klarna |

# Hemsida och maillista

## Hemsida

Det enklaste är om hemsidan görs på samma plattform som webshoppen, se nedan. Wordpress och WooCommerce verkar vara en enkel lösning som man snabbt kan komma igång med.


## Maillista

SFF kansli underhåller en maillista (ultimateklubbar@frisbeesport.se). Adresser finns även i idrottonline. Det bästa hade varit om klubbarna själva kunde logga in och uppdatera sina kontaktuppgifter. Det borde finnas en plug-in will wordpress där klubbar kan få login att underhålla sina kontaktuppgifter. Ett alternativ kan också vara att använda Wordpress feature multisite som gör det möjligt att sätta upp flera WP-siter i en installation. En site skulle kunna vara ett intranet för Ultimateklubbarna.


# Ekonomisystem och Webshop

# Nuläge

## Huvudbok

Bokföring görs manuellt i SpeedLedger av kansliet.

## Inbetalningar / kundfakturor

SUF har idag ett bankgiro som används för inbetalningar. Vissa landslag har ordnat med Swish men detta är inte kopplat till SUF:s bankkonto. Det finns en lösning i idrottonline för att generera fakturor för medlemsavgifter som skickas till Fortnox men den används inte.

## Utbetalningar / leverantörsfakturor

Alla utbetalningar görs idag från internetbanken av kansliet och bokförs manuellt. Vid behov av utbetalningar mailas kansliet som sedan sköter hanteringen.

## Ekonomirapporter

Endast kansliet kan ta ut ekonomirapporter idag.


# Krav på framtida lösning

## Introduktion / terminologi

I ekonomisystemet hanteras den löpande bokföringen och det finns även stöd för kundfakturor, leverantörsfakturor, löner etc. i moderna lösningar. Det är viktigt att de lösningar som väljs fungerar bra tillsammans och med banken (som idag är Swedbank).

I en webshop tar en organisation upp ordrar från sina kunder för olika typer av produkter. Oftast lägger kunderna de produkter de vill beställa i en kundvagn och checkar sedan ut och betalar för sin beställning. Både fysiska produkter som levereras till en kund och olika typer av tjänster/prenumerationer (som inte leveras fysiskt) säljs genom webshoppar. Den grafiska layouten går att anpassa i alla webshoppar. Tanken med att använda en webshop är att göra det enkelt att ta emot betalningar från medlemsföreningarna och medlemmarna. Betalningarna kan vara för licenser, landslag etc.

SFF har beskrivit sina [rutiner](http://styrelse.frisbeesport.se/sff-rutiner) vilka till viss del är relevanta även för oss. 

## Inbetalningar via webshop

Vi har främst behov av att ta betalt för tjänster (utan fysisk leverans) och har i dagsläget ej behov av premnumerationer (även om detta skulle kunna användas för licenser). Produkterna ska helst gå att organiseras i sortiment som olika personer kan administrera (se nedan). Vi har inte behov av rabatter eller prislistor som anpassas till respektive kund.

Idealt hade alla inbetalningar automatiskt bokförts i bökföringssystemet. Detta är förmodligen dyrt att få till om man inte kör en webshop-lösning som kommer från samma leverantör som bokföringssystemet. Alternativet är att skapa bokföringsunderlag från webshoppen eller använda uttdrag från banken.


## Inbetalningar via Bankgiro och Swish

Stöd för bankgiro ska finnas även i en framtida lösning. Inbetalningar bör gå att bokföra automatiskt. Ev. Swish bör kopplas till SUF:s bankkonto och även kopplas till bokföringen.


## Leverantörsbetalningar

En lösning där de som har behov av att göra utbetalningar (ekonomiansvarig i styrelsen, landslagsledare, projektledare, m.fl.) kan initiera utbetalningar är önskvärt. Betalningar av leverantörsfakturor bör automatiseras för att undvika dubbelarbete.


## Rapporter

Styrelsen måste ha möjlighet att själv ta ut ekonomirapporter. De som är ansvariga för ta in olika typer av avgifter måste själva kunna se vilket som har betalat. Det ska också vara möjligt att enkelt se vilka intäkter och kostander som olika projekt (landslag mm.) har haft. En lösning där transaktioner märks med projekt är en lösning och separata konton skulle också kunna användas.


## Roller och rättigheter

Det bör vara möjligt att låta olika personer kunna administrera olika delar av sortimentet i webshoppen. Ansvarig för respektive landslag måste kunna se sina egna inbetalningar. Det behövs en funktion där olika attestflöden används beroende på beloppen på leverantörsfakturorna.


# Webshop-lösningar

## Alternativ

* Wordpress med eCom plugin som WooCommerce (båda Open Source)
* Magento (Open Source)
* Shopify (kommersiell, $29-/månad)
* Webshop från Fortnox eller Speedledger - utreds ej närmare här
* CRM lösning - en lösning som hanterar relationen med sina kunder/medlemmar. SalesForce har t.ex. en rabatterad lösning för non-profits. Detta alternativ utreds inte närmare här (men skulle kunna vara ett alterntiv om vi vill bygga en lösning för att hantera marknadsföring, kampanjer etc.).

Nedan beskrivs kort de olika altertnativen. Fokus ligger främst på roller och rättigheter eftersom det är inom detta område vi har lite högre krav.


### WooCommerce

Verkar inte ha stöd för att olika personer hanterare olika delar av sortimentet i standardlösningen. Det kan finnas plug-ins för detta och det verkar också gå att ha en multi-store setup. Mer info [här](https://docs.woocommerce.com/document/roles-capabilities/).


### Magento

Inte heller Magento tycks vid en första check ha stöd för olika administratörer för olika delar av sortimentet. Mer info [här](https://docs.magento.com/m1/ce/user_guide/store-operations/admin-overview.html). Multi-store setup [nämns här också](https://devdocs.magento.com/guides/v2.2/config-guide/multi-site/ms_over.html).


### Shopify

Inget om flera shop admins. Mer info [här](https://help.shopify.com/en/manual/intro-to-shopify/shopify-admin/shopify-admin-overview).

### Multi-store / Multi-vendor store

Eftersom ingen av de lösningar som undersökts tycks ha stöd för flera administratörer/shop-managers har jag börjat titta på en s.k. multi-store lösning. Hittade ett Quora inlägg [här](https://www.quora.com/I-want-a-website-where-people-can-make-their-stores-and-sell-their-products-My-website-will-be-just-like-a-shopping-mall-where-different-sellers-will-add-their-products-to-stores-What-are-any-open-source-CMS-or-platforms-which-provide-this-functionality). WooCommerce nämns som ett alternativ som har en multi-store plugin.

## Kostnad

Med en Open Source lösning är mjukvaran gratis (om man installerar den själv och inte väljer att köpa support). Det behövs någon form av hosting och betalningslösningarna tar också ut en avgift.

### Hosting

AWS är ett alternativ att köpa en server i molnet. AWS används idag för att hantera domänen ultimatesweden.se (ligger under ett konto som SFF äger). Det enklaste är förmodligen att skaffa ett eget konto för SUF hos AWS (den enda som krävs är ett kreditkort). En server hos AWS (EC2 t3.medium) kostar $400/år.

### Betalningslösning

För att få en exakt kostnad behöver vi begära in offerter från några leverantörer. Här är grov 
uppskattning för betaltjänster som tar kreditkort baserat på info jag hittat på nätet:
* startavgift - 5.000 SEK
* månadskostnad - 600-700 SEK
* transsaktionsavgift - 3%

Ett annat alternativ är att använda PayPal som tar c:a 3% + 3,25SEK (inga uppsättnings eller fasta kostnader).

Shopify har en egen betalningslösning som kostar 2,9% + $0,3 per transaktion.


### Klarna

En vanlig betalningslösning är klarna och dom har en WooCommerce plug-in. Klarna Checkout är nog den variant som passar SUF bäst. Utbetalningar från Klarna görs i klumpsummor med en fördröjning som beror på vilket avtal man har. Mer info finns i 
[Klarnas FAQ](https://www.klarna.com/se/foretag/butikssupport/bokforing-utbetalning/nar-far-vi-utbetalningen-var-forsaljning/)


# Ekonomisystem

Två ekonomisystem som många använder är Fortnox oxh SpeedLedger. RF har avtal med både och SFF har valt att köra Fortnox. Dessa (och ev. andra alternativ) kommer att utvärderas mot de krav som listats ovan. 



# Länkar

* [The Cheapest Possible Way to Launch an Ecommerce Store](https://ecommerce-platforms.com/ecommerce-selling-advice/the-cheapest-possible-way-to-launch-an-ecommerce-store)
* [AWS priser för en server](https://aws.amazon.com/ec2/pricing/on-demand/)
* [DIBS](https://www.dibs.se/woo-commerce)
* [Klarna vs SveaWebPay](http://driva-webshop.se/klarna-eller-sveawebpay/)
* [PayPal kostnader](https://www.paypal.com/se/webapps/mpp/paypal-fees)
* [Shopify kostnader](https://www.shopify.com/pricing)

* [Klarna WooCommerce plug](https://woocommerce.com/products/klarna-checkout/) - Klarna länkar till denna sida

* [SFF-rutiner](http://styrelse.frisbeesport.se/sff-rutiner) 
