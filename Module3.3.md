**Common Reporting Framework**

The IPCC requires all national reports to be consistent with their reporting framework - referred to as the Common Reporting Framework, or CRF. The CRF includes categorisation of emission sources and sinks by sector, and is supported with a Microsoft Excel spreadsheet. The outputs of the FLINT will be able to be reconciled against the CRF; however in general the output will be finer than is required for the CRF (i.e. pools may need to be aggregated for reporting purposes). While it is possible for the FLINT to automatically generate reports consistent with the CRF, it would remove some of the versatility of the FLINT, and would also bind up-dates to the system each time the CRF was altered. More information on the CRF can be found at www.ipcc-nggip.iges.or.jp/public/gl/guidelin/ch1ri.pdf

**CO2 and Non-CO2 Reporting**

The FLINT is fully configurable to report on both CO2 and non-CO2 emissions. This is managed through the pool process, where pools can include any value. However, the FLINT does not yet restrict transfers from carbon to non-carbon pools – this is required to be restricted through the implementation of modules.
Of note, due to the mass balance requirements, the FLINT must include a pools, from which carbon (e.g. CO2 & CH4) and non-carbon pools (e.g. N2O) can draw values from.

**Land Area Matrices**

TBC

**Generic data sources**
**_Forest Biomes_**

The IPCC provides Tier 1 figures of above and below ground biomass by forest type (see Table 4.8, Chapter 4, Volume 4). By combining these default estimates with estimates of the area cleared by forest type obtained through remote sensing, it is possible to readily obtain a Tier 1 model of deforestation.
While there are numerous forest mapping tools available, such as the WWF terrestrial ecosystems, these are not well aligned with the IPCC biomass figures. For this reason, it is recommended that the FAO Global Ecological Zones be used for this purposes, as this will be consistent with the IPCC approach.
Originally released in 2001 and updated in 2010, the GEZ offers a map of the world’s forest zones, reflecting the IPCC categories (Table 1). Noting that these forest zones are not maps of forest cover. Separate forest cover maps will be necessary for monitoring deforestation.
The GEZ are Available at: data.fao.org/map?entryId=2fb209d0-fd34-4e5e-a3d8-a13c241eb61b&tab=about

| Name        | Criteria                                 | Name                            | Code  | Criteria                                                    |
| ----------- | ---------------------------------------- | ------------------------------- | ----- | ----------------------------------------------------------- |
| Tropical    | All months                               | Tropical rain forest            | TAr   | Wet: 0 – 3 months dryb. When dry period, during winter      |
| Tropical    | without frost: in marine areas over 18°C | Tropical moist deciduous forest | TAwa  | Wet/dry: 3 – 5 months dry, during winter                    |
| Tropical    | without frost: in marine areas over 18°C | Tropical dry forest             | TAwb  | Dry/wet: 5 – 8 months dry, during winter                    |
| Tropical    | without frost: in marine areas over 18°C | Tropical shrubland              | TBSh  | Semi-Arid: Evaporation > Precipitation                      |
| Tropical    | without frost: in marine areas over 18°C | Tropical desert                 | TBWh  | Arid: All months dry                                        |
| Tropical    | without frost: in marine areas over 18°C | Tropical mountain systems       | TM    | Approximate > 1000 m altitude (local variations)            |
| Subtropical | Eight months                             | Subtropical humid forest        | SCf   | Humid: No dry season                                        |
| Subtropical | or more over 10°C                        | Subtropical dry forest          | SCs   | Seasonally Dry: Winter rains, dry summer                    |
| Subtropical | or more over 10°C                        | Subtropical steppe              | SBSh  | Semi-Arid: Evaporation > Precipitation                      |
| Subtropical | or more over 10°C                        | Subtropical desert              | SBWh  | Arid All months dry                                         |
| Subtropical | or more over 10°C                        | Subtropical mountain systems    | SM    | Approximate > 800-1000 m altitude                           |
| Temperate   | Four to eight months                     | Temperate oceanic forest        | TeDo  | Oceanic climate: coldest month over 0°C                     |
| Temperate   | Four to eight months                     | Temperate continental forest    | TeDc  | Continental climate: coldest month under 0°C                |
| Temperate   | Four to eight months                     | Temperate steppe                | TeBSk | Semi-Arid: Evaporation > Precipitation                      |
| Temperate   | Four to eight months                     | Temperate desert                | TeBWk | Arid: All months dry                                        |
| Temperate   | Four to eight months                     | Temperate mountain systems      | TM    | Approximate > 800 m altitude                                |
| Boreal      | Up to 3 months over 10°C                 | Boreal coniferous forest        | Ba    | Vegetation physiognomy: coniferous dense forest dominant    |
| Boreal      | Up to 3 months over 10°C                 | Boreal tundra woodland          | Bb    | Vegetation physiognomy: woodland and sparse forest dominant |
| Boreal      | Up to 3 months over 10°C                 | Boreal mountain systems         | BM    | Approximate > 600 m altitude                                |
| Polar       | All months below 10°C                    | Polar                           | P     | Same as domain level                                        |

Soils
As with the forest biomes, it is necessary to have a spatial representation of soil to estimates of their emissions can be completed. There are multiple maps that are available for mapping the soils. The FAO World Resource Base Map contains information on soils, which can be classified up into the IPCC reporting categories (see the below table).
This is available for download at: www.fao.org/soils-portal/soil-survey/soil-maps-and-databases/other-global-soil-maps-and-databases/jp/

| FAO WRB Class  | IPCC Class     |
| -------------- | -------------- |
| Acrisol AC     | LAC Soils      |
| Albeluvisol AB | HAC Soils      |
| Alisol AL      | HAC Soils      |
| Andosol AN     | Volcanic Soils |
| Anthrosol AT   | LAC Soils      |
| Arenosol AR    | Sandy Soils    |
| Calcisol CL    | HAC Soils      |
| Cambisol CM    | HAC Soils      |
| Chernozem CH   | HAC Soils      |
| Cryosol CR     | LAC Soils      |
| Durisol DU     | LAC Soils      |
| Ferralsol FR   | LAC Soils      |
| Fluvisol FL    | LAC Soils      |
| Gleysol GL     | Wetland Soils  |
| Gypsisol GY    | HAC Soils      |
| Histosol HS    | Organic Soils  |
| Kastanozem KS  | HAC Soils      |
| Leptosol LP    | HAC Soils      |
| Lixisol LX     | LAC Soils      |
| Luvisol LV     | HAC Soils      |
| Nitisol NT     | LAC Soils      |
| Phaeozem PH    | HAC Soils      |
| Planosol PL    | LAC Soils      |
| Plinthosol PT  | LAC Soils      |
| Podzol PZ      | Spodic Soils   |
| Regosol RG     | HAC Soils      |
| Solonchak SC   | LAC Soils      |
| Solonetz SN    | HAC Soils      |
| Stagnosol ST   | LAC Soils      |
| Technosol TC   | LAC Soils      |
| Umbrisol UM    | HAC Soils      |
| Vertisol VR    | HAC Soils      |

As an alternative, the ISRIC (World Soil Information) has produced a global soils map that is also consistent with the IPCC guidelines. This data is freely available for education and non-commercial purposes – however, written consent is needed for any commercial use of the product.
These are available at: www.isric.org/data/ipcc-default-soil-classes-derived-harmonized-world-soil-data-base-ver-11.