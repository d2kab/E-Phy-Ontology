# E-Phy-Ontology
Le catalogue E-Phy contient l'ensemble des données des produits (produits phytopharmaceutiques, matières fertilisantes et supports de culture, adjuvants, produits mixtes et mélanges) couverts par une Autorisation de Mise sur le Marché (AMM) ou un permis de commerce parallèle. En France, les décisions d’AMM et de permis sont délivrées par l’ANSES depuis juillet 2015. L’agence partage ce catalogue via [l’application web E-Phy](www.ephy.anses.fr) qui est un reflet de l’état actuel des autorisations de produits et qui permet de faire des recherches pour retrouver un produit par numéro AMM, usage ou composition. Ces données servent principalement aux professionnels du secteur pour savoir si un produit est autorisé ou pour connaître les substances actives composant un produit, les sociétés détentrices d’autorisations pour la commercialisation de ces produits ainsi que leurs usages.

![Schema UML simplifié ](https://github.com/syphax-bouazzouni/EPHY-TEST/blob/main/uml.png)

La ressource ITAB est un autre ‘catalogue’ sous le nom de [Guide des produits de protection des cultures utilisables en Agriculture Biologique](www.itab.asso.fr/downloads/com-intrants/guide-protection-plantes6.pdf) en France produit par L’Institut Technique de l’Agriculture Biologique (ITAB) qui maintient, de manière distincte de l’ANSES, une liste des produits de protection des cultures, utilisables dans le cadre de la production biologique. Cependant, tous les produits du guide ITAB (version de septembre 2014 en ligne) sont inclus dans la base de données E-Phy dénotés avec la propriété “mentions-autorisées=utilisable en agriculture biologique”.
## Lien des ontologies produites
* [**ontologie E-PHY sans instances**](https://github.com/d2kab/E-Phy-Ontology/blob/main/ontologies%20produites/ephy-v1.1.owl)
* [**ontologie E-PHY avec instances**](http://agroportal.lirmm.fr/ontologies/E-PHY)
* [**ontologie ITAB avec instances**](http://agroportal.lirmm.fr/ontologies/ITAB)

## Plan du dépot
* **Dossier des fichiers sources (version octobre 2020):** 
* Fichier **UML.drawio** , conteant le diagramme de classe de la ressource d'origine (a ouvrir avec [draw.io](http://draw.io/))
* **Dossier des fichiers d'alignement:** Contient __les fichiers excel__ des equivalances trouver entre les elements d'origine et ceux d'autre ontologie
* **Dossier des fichiers utilisé en instanciation:** 
  * __talend.rar__ : le projet Talend utlisé pour les praitraitments dans données d'orgine , a extraire et importer dans Talend
  * Pour chaque element dans la base de connassiance (Intrant , Usage , Substance , Culutre preconisé ) on a dossier qui contient :
    1. Fichier source **(Input Talend)**
    2. Fichiers prétraités **(Output Talend)** 
    3. Script Cellfie **(Pour l'importation avec Protégé)** 
* **Dossier des ontologies produites** 
* **Dossier des requetes SPARQL**  qui valorisent la sémantique et les alignements de l'ontologie produite
