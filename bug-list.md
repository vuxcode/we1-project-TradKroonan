# Bug List

> Make a list of the things that don't work as expected. Keep a list of things that you have fixed and try to document how you solved them.
1. <a>-tag under själva review-blocket
  
**Löst!**
Menyn kommer inte upp på dem andra sidorna 
  - Problemet låg i att jag bara tittade på film-sidan och saknade alla kod för menyn medan alla andra sidor hade kod och meny.
    Så det var egentligen inget större fel/bugg

En liten glipa i botten mellan social och absoluta botten på hemsidan
  - Löste detta med vertical-align: bottom (används inte längre)


Menyn krymper inte rätt. vid en viss storlek på skärmen hoppar menyn 
  - Valde sedan att använda detta som en feature för mindre skärmar, 
    men detta berodde på att ramarna på knapparna behöll bredden 
    och därmed krympte inte allt med skärmen och behövde sedan ta mer höjd för att behålla bredden.

Knapparna täcks inte helt av en länk. Testade samma princip som knapparna i "Latest-review"
  - Strukturerade om allt. Först till att <a> täckte hela <li> vilket inte var godkänt av validator. 
    Detta ändrades sedan till ursprungsformatet men med hjälp av white-space: 
    pre; för att lösa radbrytningen från knappen för “kontakt info”.

Latest-review beter sig skumt. Lägger sig inte riktigt där jag vill ha den.
  - Vertical-align:top;
  - Används på flera ställen där jag hade samma problem

Anchor-tag täcker mer i sociala medier än vad den borde
  - Hårdkodar height-value till att vara något som är väldigt likt storleken på “sociala media” - bilderna. Inte perfekt men tillräckligt

