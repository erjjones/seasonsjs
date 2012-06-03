#Welcome to **Seasons.js**
*A JavaScript library which returns the season of the client*

###Factors
* __Date__ - Month Day
* __Hemisphere__ - Northern or Southern
* __CalendarType__ - Meteorological or Astronomical
* __SeasonType__ - Calendar or Special

###Estimate Factors
* __CountryCode__ - US
* __Language-Culture__ - en-US

###Season Forumla
* Date + CalendarType + SeasonType + Hemisphere = Season

###Estimated Season Formulas
* Date + CalendarType + SeasonType + CountryCode = Estimated Season
* Date + CalendarType + SeasonType + Language-Culture = Estimated Season

###Default Season Formulas
* Date + {CalendarType: Meteorological} + {SeasonType: Calendar} + {Hemisphere: Northern} = Season

###Default Estimated Season Formulas
* Date + {CalendarType: Meteorological} + {SeasonType: Calendar} + {CountryCode: US} = Estimated Season
* Date + {CalendarType: Meteorological} + {SeasonType: Calendar} + {Language-Culture: en-US} = Estimated Season

###Meteorological Calendar Season Dates
|                                   |                             |
|:----------------------------------|:----------------------------|
| **Northern Hemisphere**                                         |
| Spring                            | 1 March to 31 May           |
| Summer                            | 1 June to 31 August         |
| Autumn                            | 1 September to 30 November  |
| Winter                            | 1 December to 29 February   |
|                                                                 |
| **Southern Hemisphere**                                         |
| Spring                            | 1 September to 30 November  |
| Summer                            | 1 December to 29 February   |
| Autumn                            | 1 March to 31 May           |
| Winter                            | 1 June to 31 August         |
|                                                                 |

###Astronomical Calendar Season Dates
|                                   |                             |
|:----------------------------------|:----------------------------|
| **Northern Hemisphere**                                         |
| Spring                            | 21 March to 20 June         |
| Summer                            | 21 June to 20 September     |
| Autumn                            | 21 September to 20 December |
| Winter                            | 21 December to 20 March     |
|                                                                 |
| **Southern Hemisphere**                                         |
| Spring                            | 21 September to 20 December |
| Summer                            | 21 December to 20 March     |
| Autumn                            | 21 March to 20 June         |
| Winter                            | 21 June to 20 September     |
|                                                                 |

###Calendar Seasons
|                                   |
|:----------------------------------|
| **Traditional Seasons**           |
| Spring                            |
| Summer                            |
| Autumn                            |
| Winter                            |
|                                   |

###Special Seasons 
|                                   |
|:----------------------------------|
| **Tropical Seasons**              |
| Dry                               |
| Wet                               |
|                                   |
| **Storm Seasons**                 |
| Thunderstorm                      |
| Supercell                         |
| Downburst                         |
| Lightning                         |
| Tornado                           |
| Waterspout                        |
| Tropical cyclone (Hurricane)      |
| Extratropical cyclone             |
| Winter storm                      |
| Blizzard                          |
| Ice storm                         |
| Dust storm                        |
| Firestorm                         |
| Cloud                             |
|                                   |
*__Note__ special seasons will not be included in seasons.js until future releases.*


###Southern Hemisphere Countries

*The following countries are either entirely or mostly in the Southern Hemisphere per [Wikipedia](http://en.wikipedia.org/wiki/Southern_Hemisphere).*

*We will only key off of this list for Southern Hemisphere otherwise it will default to Northern Hemisphere.*
|                                   | Country Code                 |
|:----------------------------------|:-----------------------------|
| **Africa**                                                       |
| Angola                            |                              |
| Botswana                          |                              |
| Burundi                           |                              |
| Comoros                           |                              |
| Lesotho                           |                              |
| Madagascar                        |                              | 
| Malawi                            |                              |
| Mauritius                         |                              |
| Mozambique                        |                              |
| Namibia                           |                              |
| Rwanda                            |                              |
| Seychelles                        |                              |
| South Africa                      |                              | 
| Swaziland                         |                              |
| Tanzania                          |                              |
| Zambia                            |                              | 
| Zimbabwe                          |                              |
| Democratic Republic of the Congo  |                              |
| Gabon                             |                              |
| Republic of the Congo             |                              |
| **Asia**                                                         |
| East Timor                        |                              | 
| Indonesia                         |                              | 
| **Australia**                                                    |
| Australia                         |                              |
| Papua New Guinea                  |                              |
| **South America**                                                |
| Argentina                         |                              | 
| Bolivia                           |                              |
| Chile                             |                              |
| Paraguay                          |                              |
| Peru                              |                              | 
| Uruguay                           |                              |  
| Brazil                            |                              |  
| Ecuador                           |                              | 
| **Pacific Ocean**                                                |
| American Samoa                    |                              |   
| Cook Islands                      |                              |
| Easter Island                     |                              |
| Fiji                              |                              |
| French Polynesia                  |                              |
| Galapagos Islands                 |                              |
| Jarvis Island                     |                              |
| Juan Fernandez Islands            |                              |
| Nauru                             |                              |
| Territory of New Caledonia        |                              | 
| New Zealand                       |                              |
| Niue                              |                              |
| Kermadec Islands                  |                              | 
| Pitcairn Islands                  |                              |
| Samoa                             |                              |
| Solomon Islands                   |                              | 
| Swains Island                     |                              |
| Tokelau                           |                              | 
| Tonga                             |                              |
| Tuvalu                            |                              | 
| Vanuatu                           |                              |
| Wallis and Futuna                 |                              |
| **Atlantic Ocean**                                               |
| Falkland Islands                  |                              |
| Saint Helena                      |                              |
| Tristan da Cunha                  |                              | 
| **Indian Ocean**                                                 |
| British Indian Ocean Territory    |                              | 
| Mayotte                           |                              |
| Reunion                           |                              | 
| **Southern Ocean**                                               |
| Antarctic islands                 |                              |
| Bouvet Island                     |                              | 
| Kerguelen Islands                 |                              |
| New Zealand SubAntarctic Islands  |                              |  
| Saint Paul and Amsterdam Island   |                              |
| South Georgia                     |                              |
| South Orkney Islands              |                              | 
|                                   |                              |

###Sources: 
- http://www.calendar-365.com/
- http://en.wikipedia.org/wiki/Season
- http://en.wikipedia.org/wiki/Southern_Hemisphere