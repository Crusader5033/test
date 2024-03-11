# test
XSRF:Musí se vygenerovat XSRF token, který se budev porovnávat.Takže je potřeba vytvořit metody na vygenerovani tokenu a jeho overeni. To vse v gruyere.py v classe GruyereRequestHandler.Následně v kazde metode kde se neco deje napr. _DoDeletesnippet.Stejne tak ve formu musim posilat unikat token který se bude porovnavat. Neumim python tudíz implementace v kodu neni mozna.
Jsou tam v GruyereRequestHandler nejake metody s komentem, a _DoNewsnippet2 kde je taky koment a nejakej ten kod.Takze chill.Tokeny jsou nyní svázány s konkrétními akcemi, což brání jejich opakovanému použití pro různé požadavky.Mel bych se vyhnout jsem se neúčinným opatřením, jako je kontrola Referer hlavičky nebo kopírování cookies do skrytých polí ve formuláři.
Slo by to pouziy v deletesnippet, login apod.

Stored XSS:Je to whitelist spravnych reseni ale bylo by potreba rozsirit. Kontrolovat vsechny url,a css relace.
Reflected XSS: JSON nesmi se interpretovat jako HTML
