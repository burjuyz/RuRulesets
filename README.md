
# RU rulesets for Sing-Box



Атообновляемые (каждые 3 дня) списки адресов сконвертированные в формат ruleset которые могут применяться в приложениях с ядром Sing-Box выше 1.8.0
## Описание
В этих файлах содержатся:

Списки популярных блокировщиков рекламы (uBlock Origin, adBlock, Adguard) собранных автором Schakal [4PDA](https://4pda.to/forum/index.php?showtopic=275091&st=8000#Spoil-89665467-4) 

Списки блокировки всех известных трекеров собранных автором Sakib Mahmud [Github](https://github.com/SM443/Pi-hole-Torrent-Blocklist)  

Списки заблокированных сайтов в РФ [Antifilter Download](https://community.antifilter.download)

Списки заблокированных сайтов в РФ [Antizapret](https://github.com/zapret-info/z-i)


Для генерации была использована библиотека от Dunamis4tw [Github](https://github.com/Dunamis4tw/generate-geoip-geosite)
## Прямые ссылки

добавьте в свой конфиг

https://github.com/burjuyz/RuRulesets/raw/main/ruleset-domain-adaway_alive_hosts_mail_fb.srs

https://github.com/burjuyz/RuRulesets/raw/main/ruleset-domain-torrent_websites.srs

https://github.com/burjuyz/RuRulesets/raw/main/ruleset-domain-torrent_trackres.srs

https://github.com/burjuyz/RuRulesets/raw/main/ruleset-domain-antifilter_community.srs

https://github.com/burjuyz/RuRulesets/raw/main/ruleset-ip-antifilter_allyouneed.srs

https://github.com/burjuyz/RuRulesets/raw/main/ruleset-ip-antizapret.srs

https://github.com/burjuyz/RuRulesets/raw/main/ruleset-domain-antizapret.srs
## Пример

```javascript
    {
        "tag": "torrent_websites",
        "type": "remote",
        "format": "binary",
        "url": "https://github.com/burjuyz/RuRulesets/raw/main/ruleset-domain-torrent_websites.srs",
        "download_detour": "direct",
        "update_interval": "168h0m0s"
      },
```

