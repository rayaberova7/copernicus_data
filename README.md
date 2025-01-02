# Codes pour accéder aux données Copernicus

```{bash}
git clone https://github.com/rayaberova7/copernicus_data.git
cd copernicus_data
source ./setup.sh
```

## Images SENTINEL2

Notebook sentinelhub/data_download_process_request.ipynb pour récupérer une image Sentinel2 incluse dans le polygone Europe (tracé à la main sur le bowser Copernicus) et l'enregistrer en tiff. L'image se composera de toutes les bandes, d'un filtre nuage qui va reconstruire une image à partir des images les moins nuages sur la fenêtre de temps demandée (ici 1er au 30 janvier 2023).

### Prérequis

Il faut tout d'abord se créer un compte sur le [site Copernicus](https://dataspace.copernicus.eu/).
Aller dans Your profile --> Dashboards --> Sentinel Hub --> User settings --> OAuth client --> Create et enregistrer l'identifiant et le secret. Ils seront demandés pour récupérer une image Sentinel.
