# seznamds

![Logo](seznamds.svg?raw=true)

Debian package containing a directory of Czech DataBox (Datová schránka) identifiers.

## Installed files

| File | Description |
|------|-------------|
| `/var/lib/seznamds/seznam_ds.xml` | All DataBoxes |
| `/var/lib/seznamds/seznam_ds_po.xml` | Legal entities (PO) |
| `/var/lib/seznamds/seznam_ds_pfo.xml` | Natural persons doing business (PFO) |
| `/var/lib/seznamds/seznam_ds_ovm.xml` | Public authorities (OVM) |

## Data format

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
</list>
```

## AppStream metadata

AppStream metainfo is shipped at `/usr/share/metainfo/cz.vitexsoftware.seznamds.metainfo.xml`.
The application icon is installed at `/usr/share/icons/hicolor/scalable/apps/seznamds.svg`.

## Installation

```bash
sudo apt install lsb-release curl apt-transport-https

sudo curl -fsSL https://repo.vitexsoftware.com/KEY.gpg -o /usr/share/keyrings/vitexsoftware-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/vitexsoftware-archive-keyring.gpg] https://repo.vitexsoftware.com $(lsb_release -sc) main" | sudo tee /etc/apt/sources.list.d/vitexsoftware.list
sudo apt update

sudo apt install seznamds
```
