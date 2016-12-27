#Documentation Map-Component

###Exemple
[Cliquez ici](https://greg-klein.github.io/map-component/) pour voir un exemple d'utilisation du composant.

###Description
Ce composant permets d'afficher un fond de carte Openlayers 3 sur lequel seront ajoutées des zones géographiques provenant d'un flux GeoJson.

---
###Attributs

| Nom | Type | Description | Facultatif | Valeur par défaut |
|-----|------|-------------|------------|-------------------|
| geojson-service | String | Url du service fournissant le GeoJson | Non |
| map-service | String | Url du service de carte (ex: mapbox, bing, …) | Oui |
| zoom | Boolean | Si présent, zoom directement sur les points/zones lors du chargement de la map | Oui | Non présent / false |
| show-coords | Boolean | Si présent, affiche les coordonnées du curseur | Oui | false |
| default-zoom | Number | Définit le zoom par défaut si l'attribut **zoom** n'est pas présent | Oui | 2 |
| default-center-long | Number | Définit la longitude du centre de la map si l'attribut **zoom** n'est pas présent | Oui | 0 |
| default-center-lat | Number | Définit la latitude du centre de la map si l'attribut **zoom** n'est pas présent | Oui | 0 |


---
###Utilisation

Le composant s'insère dans une page de cette manière:

```html
<map-component geojson-service="http://url/du/service" {...attributs...}></map-component>
```