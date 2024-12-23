# DVB設定ファイル (DVB Configurations for ISDB)

[DVB Configurations for ISDB][link_org]に対してBS帯域再編（トランスポンダ間の移動）を反映させたものです。
また、以下のファイルを追加しています。

* LNB電源供給用ISDB-S用設定ファイル`dvbv5_channels_isdbs_lnb.conf`の追加
* DVB-C用設定ファイル`dvbv5_channels_dvbc.conf`の追加

## 使用方法

```console
dvbv5-zap -a <adapter#> -c dvbv5_channels_isdbt.conf -r -P <channel>
dvbv5-zap -a <adapter#> -c dvbv5_channels_isdbs.conf -r -P <channel>
dvbv5-zap -a <adapter#> -c dvbv5_channels_isdbs_lnb.conf -r -P <channel>
dvbv5-zap -a <adapter#> -c dvbv5_channels_dvbc.conf -r -P <channel>
```

[link_org]: https://github.com/Chinachu/dvbconf-for-isdb
