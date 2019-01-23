Moduly

Když restartujete Pythoní interpretr, definice, které jste vytvořili (funkce a
proměnné), jsou ztraceny. Pokud tedy chcete napsat delší program, bude lepší
použít textový editor, aby bylo možné dopředu připravit vstup pro Pythoní
interpreter a pustit jej ze souboru. Toto je známo jako vytváření *skriptu*. S
narůstající délkou programu je vhodné jej rozdělovat do souborů pro snazší
údržbu. Tento postup umožňuje i použití stejné funkce v různých programech bez
nutnosti ji pokaždé definovat znovu.

V Pythonu lze vložit definice do souboru a používat je ve skriptu či
interaktivní instanci interpreteru. Takový soubor se jmenuje *modul*. Definice v
module mohou být *importovány* do jiných modulů či do *hlavního* modulu (soubor
proměnných, ke kterým lze přístupit ze skriptu spuštěném na nejvyšší úrovni, či
z interkativního módu).

Module je soubor obsahující Pythoní definice a výrazy. Název souboru se skládá
ze jména modulu a připony :file:`.py`. Zevnitř modulu je jeho název (jakožto
řetězec) přístupný pod proměnnou ``__name__``. Jako příklad, vytvořte ve svém
oblíbeném textovém editoru soubor s názvem :file:`fibo.py` v aktuálním adresáři
s nádledujícím obsahem::

Nyní po spuštení interpreteru můžete importovat modul fibo následujícím
příkazem::

Tímto způsobem nedostaneme funkce deivnované ve ``fibo`` přimo do aktuálního
modulu, ale dostaneme je do modulu jménem ``fibo``. Přes jméno modulu se tedy
můžete dostat k jeho funkcím::

Pokud používáte danou funkci často, můžete si ji uložit do lokální proměnné::

