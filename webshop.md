# Krav

## Introduktion / terminologi

I en webshop tar en organisation upp ordrar från sina kunder för olika typer av produkter. Oftast lägger kunderna de produkter de vill beställa i en kundvagn och checkar sedan ut och betalar för sin beställning. Både fysiska produkter som levereras till en kund och olika typer av tjänster/prenumerationer (som inte leveras fysiskt) säljs genom webshoppar. Den grafiska layouten går att anpassa i alla webshoppar.

## Produkter, sortiment och prissättning

Vi har främst behov av att sälja tjänster (utan fysisk leverans) och har ej behov av premnumerationer. Produkterna ska organiseras i sortiment som olika personer kan administrera (se nedan). Vi har inte behov av rabatter eller prislistor som anpassas till respektive kund.

## Roller och rättigheter

Det bör vara möjligt att låta olika personer kunna administrera olika delar av sortimentet. T.ex. skulle ansvarig för respektive landslag administrera sina egna betalningar.

## Redovisning

Idealt hade alla betalningar automatiskt bokförts i bökföringssystemet. Detta är förmodligen dyrt att få till om man inte kör en webshop-lösning som kommer från samma leverantör som bokföringssystemet. Alternativet är att skapa bokföringsunderlag från webshoppen eller använda uttdrag från banken.
 
# Alternativ

* Wordpress med eCom plugin som WooCommerce (båda Open Source)
* Magento (Open Source)
* Shopify (kommersiell, $29-/månad)
* Webshop från Fortnox eller Speedledger
* CRM lösning - en lösning som hanterar relationen med sina kunder/medlemmar. SalesForce har t.ex. en rabatterad lösning för non-profits. Detta alternativ utreds inte närmare här (men skulle kunna vara ett alterntiv om vi vill bygga en lösning för att hantera marknadsföring, kampanjer etc.).

# Kostnad

Med en Open Source lösning är mjukvaran gratis (om man installerar den själv och inte väljer att köpa support). Det behövs någon form av hosting och betalningslösningarna tar också ut en avgift.

## Hosting

AWS är ett alternativ att köpa en server i molnet. AWS används idag för att hantera domänen ultimatesweden.se (ligger under ett konto som SFF äger). Det enklaste är förmodligen att skaffa ett eget konto för SUF hos AWS (den enda som krävs är ett kreditkort). En server hos AWS (EC2 t3.medium) kostar $400/år.

## Betalningslösning

För att få en exakt kostnad behöver vi begära in offerter från några leverantörer. Här är grov 
uppskattning för betaltjänster som tar kreditkort baserat på info jag hittat på nätet:
* startavgift - 5.000 SEK
* månadskostnad - 600-700 SEK
* transsaktionsavgift - 3%

Ett annat alternativ är att använda PayPal som tar c:a 3% + 3,25SEK (inga uppsättnings eller fasta kostnader).

Shopify har en egen betalningslösning som kostar 2,9% + $0,3 per transaktion.

# Länkar

* [The Cheapest Possible Way to Launch an Ecommerce Store](https://ecommerce-platforms.com/ecommerce-selling-advice/the-cheapest-possible-way-to-launch-an-ecommerce-store)
* [AWS priser för en server](https://aws.amazon.com/ec2/pricing/on-demand/)
* [DIBS](https://www.dibs.se/woo-commerce)
* [Klarna vs SveaWebPay](http://driva-webshop.se/klarna-eller-sveawebpay/)
* [PayPal kostnader](https://www.paypal.com/se/webapps/mpp/paypal-fees)
* [Shopify kostnader](https://www.shopify.com/pricing)
