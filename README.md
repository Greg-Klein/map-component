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
| map-service | String | Url du service de carte (ex: mapbox, bing, ...) | Oui |
| zoom | Boolean | Si présent, zoom directement sur les points/zones lors du chargement de la map | Oui | Non présent / false |
| show-coords | Boolean | Si présent, affiche les coordonnées du curseur | Oui | false |
| default-zoom | Number | Définit le zoom par défaut si l'attribut **zoom** n'est pas présent | Oui | 2 |
| default-center-long | Number | Définit la longitude du centre de la map si l'attribut **zoom** n'est pas présent | Oui | 0 |
| default-center-lat | Number | Définit la latitude du centre de la map si l'attribut **zoom** n'est pas présent | Oui | 0 |
| marker-default-color | String | Définit la couleur par défaut des éléments à afficher sur la carte (Doit être une couleur au format CSS: 'green', '#00FF00', '#0F0' ou 'rgb(0, 255, 0)') | Oui | red |


---
###Utilisation

Le composant s'insère dans une page de cette manière:

```html
<map-component geojson-service="http://url/du/service" {...attributs...}></map-component>
```

> Il est possible de passer des paramètres qui s'afficheront dans la boite modale. Pour cela, il suffit de les ajouter dans l'objet "properties" du flux GeoJson.
> Si vous ne souhaitez pas que ces paramètres s'affichent il suffit de faire débuter leur nom par le caractère "_".