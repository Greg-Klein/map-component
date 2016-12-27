#Documentation Map-Component

###Exemple
[Cliquez ici](https://greg-klein.github.io/map-component/) pour voir un exemple d'utilisation du composant.

###Description
Ce composant permets d'afficher un fond de carte Openlayers 3 sur lequel seront ajout�es des zones g�ographiques provenant d'un flux GeoJson.

---
###Attributs

| Nom | Type | Description | Facultatif | Valeur par d�faut |
|-----|------|-------------|------------|-------------------|
| geojson-service | String | Url du service fournissant le GeoJson | Non |
| map-service | String | Url du service de carte (ex: mapbox, bing, �) | Oui |
| zoom | Boolean | Si pr�sent, zoom directement sur les points/zones lors du chargement de la map | Oui | Non pr�sent / false |
| show-coords | Boolean | Si pr�sent, affiche les coordonn�es du curseur | Oui | false |
| default-zoom | Number | D�finit le zoom par d�faut si l'attribut **zoom** n'est pas pr�sent | Oui | 2 |
| default-center-long | Number | D�finit la longitude du centre de la map si l'attribut **zoom** n'est pas pr�sent | Oui | 0 |
| default-center-lat | Number | D�finit la latitude du centre de la map si l'attribut **zoom** n'est pas pr�sent | Oui | 0 |


---
###Utilisation

Le composant s'ins�re dans une page de cette mani�re:

```html
<map-component geojson-service="http://url/du/service" {...attributs...}></map-component>
```