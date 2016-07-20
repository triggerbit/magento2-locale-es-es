# magento2-locale-es-es

Traducción a idioma español (España) para Magento2

Estos ficheros se copiaron de https://crowdin.com/project/magento-2/es-ES
 
# Instalación manual
 - Descarga el zip y copia los contenidos de /src/ en la raiz de magento
 - En el directorio raiz de Magento, ejectua los siguientes comandos:
```bash
php bin/magento setup:static-content:deploy es_ES
rm -rf var/di
php bin/magento setup:di:compile
```
