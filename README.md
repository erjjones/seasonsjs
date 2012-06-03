#Welcome to **Seasons.js**
*A JavaScript library which returns the season of the client*

###Season Forumla
* Date + CalendarType + SeasonType + Hemisphere = Season

###Factors
* Date - Month Day
* Hemisphere - North or South
* CalendarType - Meteorological or Astronomical
* SeasonType - Calendar or Special

###Default Season Formulas
* Date + {CalendarType: Meteorological} + {SeasonType: Calendar} + {Hemisphere: Northern} = Season
* Date + CalendarType + {SeasonType: Calendar} + {Hemisphere: Northern} = Season
* Date + CalendarType + SeasonType + {Hemisphere: Northern} = Season

###Estimated Season Formulas
* Date + CalendarType + SeasonType + Language-Culture = Estimated Season
* Date + CalendarType + SeasonType + Country = Estimated Season

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

###Sources: 
- http://www.calendar-365.com/
- http://en.wikipedia.org/wiki/Season