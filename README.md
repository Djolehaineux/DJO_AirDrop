# DJO_AirDrop
Bienvenue sur Mon guide d'installation est de configuration pour mon mods DJO_AirDrop



## INSTALLATION
- Placer le mod a la racine de votre serveur
- Placer la key qui se trouve à l'intérieur du dossier KEY du mod dans le dossier key de votre serveur
- Déclarée le mods dans la barre de lancement de votre serveur

### Guide Configurations
`"isEnabled": 1,` Activer ou désactiver les AirDrop (1 = Activer / 0 = Désactiver)  
`"spawnInterval": 1800.0,`Interval entre chaque vague d'apparition des AirDrop (Temps definie en seconde = 30 minutes)  
`"cleanTime": 1200.0,`Temps avant suppression des AirDrop dans le monde (Temps definie en seconde = 20 minutes)  

Nom types des diférent AirDrop
```
"airdropTypes": [
    "AirDrop_T1",
    "AirDrop_T2",
    "AirDrop_T3",
    "AirDrop_T4"
    // ici vous avez la possibiliter de rejouter d'autre container exemple: SeaChest
],
```
[exemple](https://github.com/Djolehaineux/DJO-mods-collection) d'integration d'un nouveau container
Gestion des apparition des AirDrop `"airdropTypeConfigs"` 
`AirDrop_T1` Début de la configuration de l'AirDrop_T1  

`"positions"` class qui definie l'enssemble des position pour l'AirDrop_T1  
`"position"` points d'apparitions des AirDrop valeur des pos `X`, `Y`, `Z`  
`"message"` contenue du message qui sera envoyée en jeux lors de l'apparitions  

**EXEMPLE:**
```
{
    "position": [
        11872.8017578125,
        140.00003051757813,
        12555.943359375
    ],
    "message": "Alerte! Un airdrop a atterri a l' Airfield! (Krasno)"
}
```

`"spawnCountMin": 1,` quantité minimum d'AirDrop_T1 pouvent étre généré en même temps  
`"spawnCountMax": 2,` quantité maximum d'AirDrop_T1 pouvent étre généré en même temps  

---

[retourner a la collections](https://github.com/Djolehaineux/DJO-mods-collection)
