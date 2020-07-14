---
title: Regions
description: The geographic region of the visitor.
---

# Regions

The 'Regions' dimension reports the geographic region of the visitor. It is a geographic area that is smaller than a country but larger than a city. In some countries, a region is a state, province, or prefecture. In other areas, it is a constituent country, department, or metropolitan region. Using this dimension is valuable if you want insight more granular than [Countries](countries.md) but not as granular as [Cities](cities.md).

## Populate this dimension with data 

This dimension references lookup rules internal to Adobe. The lookup value is based on the IP address sent with the hit. Adobe partners with [Digital Element](https://www.digitalelement.com/) to maintain lookups between IP address and country. This dimension works out of the box for all implementations.

>[!TIP]
>
>If your organization follows stringent privacy regulations where [obfuscating IP address](/help/admin/admin/general-acct-settings-admin.md) isn't enough, you can request to disable geolocation data entirely. Contact Customer Care with the report suite ID, and request to turn off 'Geography' for the report suite.

## Dimension values

Dimension values include regions and the country that the region resides in. Example values include `"California (United States)"`, `"Tokyo (Japan)"`, or `"Sao Paulo (Brazil)"`.

## Differences between reported and actual location

Since this dimension is based on IP address, some scenarios can show a difference between reported location and actual location:

* **IP addresses that represent corporate proxies**: These visitors can appear as traffic coming through the user's corporate network, which can be a different location if the user is working remotely.
* **Mobile IP addresses**: Mobile IP targeting works at varying levels depending on the location and the network. A number of carriers backhaul IP traffic through centralized or regional points of presence.
* **Satellite ISP users**: Identifying the specific location of these users is difficult, as they typically appear to originate from the uplink location.
* **Military and government IPs**: Represents personnel traveling around the globe and entering through their home location, rather than the base or office where they are currently stationed.