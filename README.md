[![Versión mínima de PHP](https://img.shields.io/badge/php-%3E%3D%205.6.1-8892BF.svg)](https://php.net/)
[![Compatibilidad mínima con PrestaShop](https://img.shields.io/badge/prestashop-%3E%3D%201.7-8892BF.svg)](https://doc.prestashop.com/pages/viewpage.action?pageId=54264853)
[![Versión en GitHub](https://img.shields.io/github/v/release/prestaalba/ps_webhooks)](https://github.com/prestaalba/ps_webhooks/releases)

# Webhooks de PrestaShop

Envía notificaciones en tiempo real sobre eventos de PrestaShop, adjuntando los datos del objeto en formato JSON a la solicitud.

![Modulo WebHooks](https://xococode.github.io/ps_webhooks/modulo-webhooks-prestashop-n8n-integracion.webp)


## Instalación

[Descarga una versión en zip](https://github.com/prestaalba/ps_webhooks/releases) e instálala como cualquier otro módulo.

[Documentación estilo xocostudio](https://www.canva.com/design/DAGw_TmT5pg/8IovtBIumRUDg9v459ixlA/view?utm_content=DAGw_TmT5pg&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=hf039296268)

## Uso

Ve a la página de configuración del módulo en tu back office de PrestaShop. Crea tantos webhooks como necesites seleccionando la acción y la entidad de PrestaShop que quieras monitorear, y definiendo la URL de destino. Cada vez que se dispare el evento, los datos relacionados se enviarán en tiempo real mediante una solicitud **POST**, usando el siguiente ejemplo de formato JSON:

```json
{
  "action": "update",
  "entity": "Customer",
  "data": {
    "id": 42,
    "id_gender": 1,
    "id_default_group": 3,
    "id_lang": null,
    "company": "Rolige",
    "firstname": "Wilson",
    "lastname": "Alba",
    "email": "wilson@example.com",
    "passwd": "$2y$10$abc123...",
    "birthday": "1990-05-20",
    "newsletter": true,
    "optin": false,
    "active": true,
    "is_guest": false,
    "deleted": false,
    "date_add": "2023-01-15 10:00:00",
    "date_upd": "2025-08-20 05:50:00"
  }
}

```

## Contribuir

Cualquier contribución es muy bienvenida. :)

## Licencia

Este módulo se publica bajo una licencia AFL.




