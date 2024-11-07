# mojiodpadki-homeassistant
Home Assistant YAML koda za pridobivanje podatkov o odvozu smeti z Mojiodpadki.si API

# Kako pridobiti ID?
Na spletni strani **JP VOKA SNAGA** vpišite ulico in izberite hišno številko:

https://www.mojiodpadki.si/urniki/urniki-odvoza-odpadkov

Spletni obrazec vas bo preusmeril na spletni naslov v naslednji obliki:
**https://<i></i>www<i></i>.mojiodpadki.si/urniki/urniki-odvoza-odpadkov/s/<ins>xxxx</ins>**

**ID** predstavlja zadnja številka v naslovu (*zgoraj: xxxx*).

# Kako uporabiti YAML?
Vsebino **ha.yaml** kopirajte v **configuration.yaml** v [Home assistant](https://www.home-assistant.io/docs/configuration/). Besedilo **[INSERT ID]** v YAML kodi zamenjajte z ID številom, ki ste ga pridobili po zgoraj opisanih navodilih (številko vpišite med narekovaje ""), shranite spremembe in ponovno zaženite Home Assistant.

# Kako uporabiti podatke?
Home Assistant bo podatke posodobil enkrat na uro (privzeta nastavitev) in jih shranil v naslednje spremenljivke:
- sensor.mojiodpadki
- sensor.dates_for_emb
- sensor.dates_for_mko
- sensor.next_emb_date
- sensor.next_mko_date

# Splošni pogoji
Uporaba kode na lastno odgovornost. Za uporabo kode ali morebitne posledice uporabe ne prevzemam nobene odgovornosti.
