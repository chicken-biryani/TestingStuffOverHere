**Empirical Growth Model**

The empirical growth model is a forest growth module that simulates growth in carbon stock within a forest and its components through time. It is based on yield tables that presents the monthly growth increments for a forest type, as determined by the average field measurements across forest stands (i.e. empirical data). Yield refers only to aboveground biomass in [m3/mth, t/mth]. These yield tables reflect the generalised growing patterns through time, based on the prevailing environmental conditions and management of the forest types that underpin the data. Forests are measured to reflect the range of forest conditions present; as opposed to a ‘normal’ growth model that only reflects fully stocked forests.

The yield table tables increase the mass of carbon within the forest through time, and allocation tables are then used to proportion this growth to individual forest components – such as stem, leaves, fine roots, and coarse roots. Like growth, the proportional allocations will change through time as the forest matures. For example, at younger ages a larger proportion of tree growth will go into leaves than stems. The increase in carbon stock is associated with tree growth that is drawn from the atmosphere pool, ensuring mass balance.

As with all models, the empirical growth model can be calibrated to suit the data that is available, and up-dated through time. However, this is also one of its limitations, in that it requires up-dating to respond to changes in climatic conditions; whereas hybrid models do not.

**Hybrid forest growth**

Hybrid models are more complex than empirical growth models, as they use physiological responses to environmental conditions to derive relationships that can be used to predict tree growth. These models are represented as equations, or a series of equations, rather than a table. Such models are often referred to as 3-PG models (Physiological Principles in Predicting Growth). To function, these models require finer detailed data than is typically represented in empirical growth models. For example, a 3-PG model can require monthly rainfall, number of frost days, and mean daily water-vapour pressure deficit (see Landsberg & Waring 1997). The starting mass of carbon within the forest is also needed.

Under this approach, biomass partitioning is done as a proportion of aboveground biomass, which varies with age.

An advantage of hybrid models over empirical models, is that they are better suited for accounting for variation across the landscape with a more limited dataset. As only one model can be used to model growth over a variety of site conditions, where these conditions are explanatory variables in the model. Similarly, these models can be calibrated to respond to changes in management, by applying growth modifiers. More information on Hybrid growth models can be found in Brack & Richards (2002) and Waterworth et al (2007).

| Input                           | Output                 |
| ------------------------------- | ---------------------- |
| 1. Time step: monthly           | 1. Age: Age            |
| 2. Region: Province             | 2. Pool1: Stemwood     |
| 3. Species                      | 3. Pool2: Bark         |
| 4. Species: rootshoot           | 4. Pool3: Leaves       |
| 5. Age: Age                     | 5. Pool4: Course roots |
| 6. Pool1: Stemwood              | 6. Pool5: Fine roots   |
| 7. Pool2: Bark                  |
| 8. Pool3: Leaves                |
| 9. Pool4: Course roots          |
| 10. Pool5: Fine roots           |
| 11. Rainfall                    |
| 12. Minimum Temperature         |
| 13. Maximum temperature         |
| 14. Vapour Pressure Deficit     |
| 15. Soil water holding capacity |

**WOFOST**
Akin to the Hybrid forest growth model, WOFOST (World FOod STudies) is a mechanistic model that simulates crop growth on the basis of photosynthesis, respiration, and the prevailing environmental conditions. WOFOST also allocates biomass to different plant components, with the proportion varying with crop growth stage.
Unlike the hybrid growth model, WOFOST allows users to adjust the complexity of the model that is run. WOFOST allows users to model the potential production, attainable production, and actual production for a given site. WOFOST runs at daily time steps. More information on WOFOST is available at: www.wageningenur.nl/en/Expertise-Services/Research-Institutes/alterra/Facilities-Products/Software-and-models/WOFOST.htm

| Input                    | Input                    |
| ------------------------ | ------------------------ |
| 1. Time: Daily           | 1. Age: Age              |
| 2. Crop Type             | 2. Pool1: stem           |
| 3. Pool1: stem           | 3. Pool2: Leaves         |
| 4. Pool2: Leaves         | 4. Pool3: Storage organs |
| 5. Pool3: Storage organs | 5. Pool4: Roots          |
| 6. Pool4: Roots          |
| 7. Maximum temperature   |
| 8. Minimum temperature   |
| 9. Global radiation      |

**RothC**
RothC is a model for simulating the turnover of soil carbon in non-waterlogged soils under different vegetation types. It is based on the decomposition of organic matter as it relates to mean temperature and moisture, and proportion of resistant and decomposable organic material. While there are default decomposition rates in RothC, it is necessary to calibrate the model to the local conditions (Falloon & Smith 2002). RothC has a significant benefit over other soil models, such as CENTURY, as the input data is more readily available and there is also considerable overlap with the hybrid forest growth and WOFOST models. For more information on RothC, see www.rothamsted.ac.uk/sustainable-soils-and-grassland-systems/rothamsted-carbon-model-rothc.

| Input                                          | Output                      |
| ---------------------------------------------- | --------------------------- |
| 1. Time: Monthly                               | 1. Total organic carbon     |
| 2. Pool 1: Input of plant residue              | 2. Microbial biomass carbon |
| 3. Pool 2: Input of farmyard manure            |
| 4. Pool 3: Total organic carbon                |
| 5. Pool 4: Microbial biomass carbon            |
| 6. Rainfall                                    |
| 7. Open pan evaporation                        |
| 8. Mean air temperature                        |
| 9. Clay content of soil                        |
| 10. Decomposability of incoming plant material |
| 11. Soil Cover                                 |
| 12. Depth of soil layer sampled.               |

**Turnover**
Turnover is the movement from a living carbon pool to a dead carbon pool. This is due to the natural senescence of plant components, for example a deciduous forest will have near 100 per cent turnover of leaves across a year – or an annual turnover rate of 0.99. The turnover rates will vary with vegetation types, and the plant components. For example, a tree stem may have zero (0) annual turnover, while the leaves have one (1).
[To determine the volume of turnover through time, a calculation similar to the one below is carried out.
Turnover=1-(1-Turnover rate)^Time

Within the FLINT, the maximum decay rate is set at 0.99 999 999 998, and the minimum decay rate is 0.000001. These restrictions are in place to ensure there are no invalid calculations (e.g. dividing by zero).

**Decomposition**
Within the FLINT, decomposition represents heterotrophic respiration of litter and soil organic matter. The process of modelling decomposition is akin to turnover in plant material, where a proportion of biomass in litter and soil organic matter decays through time. The rates of this will vary with location based on the prevailing environmental conditions.  
As with turnover rates, within the FLINT, annual decomposition rates are limited to.....

Reference
Brack, C.L., Richards, G. P. (2002) Carbon accounting model for forests in Australia, Environmental Pollution, pp. 187-194. z
Fallon, P, Smith, P., (2002) Simulating SOC changes in long-term experiments with RothC and CENTURY: model evaluation for a regional application.
Landsberg, J.J., Waring, R.H., (1997) A generalised model of forest productivity using simplified concepts of radiation-use efficiency, carbon balance and partitioning, Forest Ecology and Management 95, pp. 209-228.
Waterworth, R.M., RIchards, G.P., Brack, C.L., Evans, D.M.W (2007) A generalised hybrid process-empirical model for predicting plantation forest growth, Forest Ecology and Management 238, pp. 231-243.