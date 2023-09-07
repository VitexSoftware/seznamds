# seznamds

Debian package that contains directory of identificatros of czech DataBoxes

* /var/lib/seznamds/seznam_ds_ovm.xml
* /var/lib/seznamds/seznam_ds_pfo.xml  
* /var/lib/seznamds/seznam_ds_po.xml  
* /var/lib/seznamds/seznam_ds.xml


Data example
------------

```xml
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<list xmlns=http://seznam.gov.cz/ovm/datafile/seznam_ds/v1 source-system="https://www.mojedatovaschranka.cz/sds" >
<box>
<id>kmn5qff</id>
<type>PFO</type>
<subtype>30</subtype>
<name>
<person>
<firstName>Mohamad</firstName>
<lastName>Abbas</lastName>
</person>
<tradeName>Mohamad Abbas</tradeName>
</name>
<ico>49483510</ico>
<address>
<city>Brno</city>
<district>Líšeň</district>
<street>Podruhova</street>
<cp>3</cp>
<co>2689</co>
<zip>62800</zip>
<addressPoint>25750577</addressPoint>
<state>CZ</state>
<fullAddress></fullAddress>
</address>
<pdz>true</pdz>
<ovm>false</ovm>
<hierarchy>
<isMaster>true</isMaster>
</hierarchy>
<idOVM></idOVM>
</box>
.
.
.
.
</list>
```

