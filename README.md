# DJO_AirDrop
Bienvenue sur Mon guide d'installation est de configuration pour mon mods DJO_AirDrop



## INSTALLATION
- Placer le mod a la racine de votre serveur
- Placer la key qui se trouve à l'intérieur du dossier KEY du mod dans le dossier key de votre serveur
- Déclarée le mods dans la barre de lancement de votre serveur

### Guide Configurations de La gestion d'apparitions des **AirDrop**
```
{
    "ConfigVersion": "1",
    "isEnabled": 1,
    "spawnInterval": 1800.0,
    "cleanTime": 1200.0,
    "isFullyInitialized": 0,
    "airdropTypes": [
        "AirDrop_T1"
        // ici vous pouvez ajoutez de nouveaux container exemple: SeaChest
    ],
    "airdropTypeConfigs": {
        "AirDrop_T1": {
            "positions": [
                {
                    "position": [
                        11872.8017578125,
                        140.00003051757813,
                        12555.943359375
                    ],
                    "message": "Alerte! Un airdrop a atterri a l' Airfield! (Krasno)"
                }
                // ici vous pouvez ajoutez de nouvel position
            ],
            "spawnCountMin": 1,
            "spawnCountMax": 2,
            "airdropLoot": {
                "categories": {
                    "Weapons_01": 1
                    // ici vous pouvez ajoutez de nouvel categories d'items
                }
            },
            "creatureCountMin": 5,
            "creatureCountMax": 10,
            "creatureTypes": [
                "ZmbF_PoliceWomanNormal",
                "Animal_CanisLupus_Grey"
                // ici vous pouvez ajoutez de nouvel créature
            ]
        }
        // ici vous pouvez ajoutez les nouveaux container
    },
```
`"isEnabled": 1,` Activer ou désactiver les AirDrop (1 = Activer / 0 = Désactiver)  
`"spawnInterval": 1800.0,`Interval entre chaque vague d'apparition des AirDrop (Temps definie en seconde = 30 minutes)  
`"cleanTime": 1200.0,`Temps avant suppression des AirDrop dans le monde (Temps definie en seconde = 20 minutes)  
`"airdropTypeConfigs"` Gestion des apparition des différent types d'AirDrop  
`"AirDrop_T1"` Début de la configuration de l'AirDrop_T1  
`"positions"` class qui definie l'enssemble des position pour l'AirDrop_T1  
`"position"` points d'apparitions des AirDrop valeur des pos `X`, `Y`, `Z`  
`"message"` contenue du message qui sera envoyée en jeux lors de l'apparitions  
`"spawnCountMin": 1,` quantité minimum d'AirDrop_T1 pouvent étre généré en même temps  
`"spawnCountMax": 2,` quantité maximum d'AirDrop_T1 pouvent étre généré en même temps  
`"airdropLoot"` class contenant la gestion d'apparitions du loot  
`"categories"` class d' appel au differente catégories d'items  
`"Weapons_01": 1,` nom de la categorie appeler pour généré le butin a l'interieur de l'AirDrop est la quantité d'items demandé  
`"creatureCountMin": 5,` quantité minimum de creature rattacher a l'airdrop  
`"creatureCountMax": 10,` quantité maximum de creature rattacher a l'airdrop  
`"creatureTypes"` class contenant les différent types de créature vous pouvez aussi bien placer des zombies que des animaux  
`"ZmbF_PoliceWomanNormal"` nom types d'un zombie  
`"Animal_CanisLupus_Grey"` nom types d'un loup  

[exemple](https://github.com/Djolehaineux/DJO-mods-collection) d'integration d'un nouveau container  



### Guide Configurations de La gestion du loot des **AirDrop**
```
    "Categories": {
        "Weapons_01": [
            {
                "item": "M4A1",
                "attachments": [
                    "M4_CQBBttstck",
                    "M4_MPHndgrd",
                    "ACOGOptic_6x",
                    "M4_Suppressor",
                    "Mag_STANAG_60Rnd"
                ]
            }
            // Ici vous pouvez rajoutez de nouveaux items
        ]
        // Ici vous pouvez rajoutez de nouvel Categories
    }
}
```
`"Categories"` class contenant les différentes catégories d'items  
`"Weapons_01"` nom de la catégories   
`"item": "M4A1"` déclarations d'un items `M4A1` nom types de l'items   
`"attachments"`  déclarations des attachemnt de l'items  
`"M4_CQBBttstck"` nom types de l'attachement  


[exemple](https://github.com/Djolehaineux/DJO-mods-collection) d'integration d'une nouvel catégorie d'items
---

[retourner a la collections](https://github.com/Djolehaineux/DJO-mods-collection)
