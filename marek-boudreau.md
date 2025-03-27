### Nomage et disposition
- Le nom de mes composants sont trop simple.
  Par exemple, Card.vue aurait pus s'appeler AlbumCard.vue

- Le fichier index.ts doit être dans le dossier scripts

### Fonctionnalités
- Aucune validation est fait dans l'ajout d'une carte dans le catalogue.
des vérifications auraient pus être ajoutés dans cette fonction qui est appelée à l'ajout d'une carte:

```javascript
function addCard(){
    addAlbum(album.value);
    confirmAlbumAddition();
}
```
---
- Le boutton pour exporter le csv toi être appellé "Exporter le CSV" et non "Télecharger".
Ce code:
```javascript
<template>
    <button type="button" class="btn btn-primary btn-lg" @click="downloadList">Télécharger</button>
</template>
```
aurait donc dût être:
```javascript
<template>
    <button type="button" class="btn btn-primary btn-lg" @click="downloadList">Exporter le CSV</button>
</template>
```