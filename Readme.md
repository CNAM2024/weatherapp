# Création d'une application web

## Initialisation

- Readme.md
- .gitignore

Nous allons créer une application Python Flask

## Etape 1

Une simple application formulaire => résultat

- installation requirements
- templates/
    - base.html
    - home.html
    - result.html
- static/
    - style.css

## Etape 2 création d'un outil interrogation d'API REST

```python
from askapi import ask_air

ask_air(apikey="XXXXXXXXXXXXXXXXXXXXXXXX",city="Toulouse")
```
```
{'CO': {'concentration': 190.26, 'aqi': 2, 'color': 'green'},
 'NO2': {'concentration': 1.63, 'aqi': 2, 'color': 'green'},
 'O3': {'concentration': 74.39, 'aqi': 98, 'color': 'yellow'},
 'SO2': {'concentration': 0.19, 'aqi': 0, 'color': 'black'},
 'PM2.5': {'concentration': 2.46, 'aqi': 7, 'color': 'green'},
 'PM10': {'concentration': 2.69, 'aqi': 2, 'color': 'green'},
 'overall_aqi': {'aqi': 98, 'color': 'yellow'}}
```

## Etape 3 intégration de l'outil dans la webapp 

Voir weather.app.py



