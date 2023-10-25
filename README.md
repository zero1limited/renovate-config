# renovate-config


```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>zero1limited/renovate-config:magento"
  ],
  "hostRules": [
    {
      "hostType": "packagist",
      "matchHost": "https://repo.magento.com",
      "username": "{{ secrets.MAGENTO_USERNAME }}",
      "password": "{{ secrets.MAGENTO_PASSWORD }}"
    },
    ...
  ],
  "constraints": {
    "php":"8.1.16"
  },
  "includeForks": true
}
```