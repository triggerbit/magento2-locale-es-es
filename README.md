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

# Instalación con composer
```bash
composer config repositories.magento2-locale-es-es vcs https://github.com/triggerbit/magento2-locale-es-es
composer require triggerbit/magento2-locale-es-es
php bin/magento i18n:pack --mode=replace -d vendor/triggerbit/magento2-locale-es-es/es_ES.csv . es_ES
php bin/magento setup:static-content:deploy es_ES
```