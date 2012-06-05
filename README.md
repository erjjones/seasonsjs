#Welcome to **Seasons.js**
*A JavaScript library which returns the season of the client*

###Basic Forumla
* Date + Hemisphere = Season

###Various Factors
* __Date__ - Month Day
* __Hemisphere__ - Northern or Southern
* __Calendar Type__ - Meteorological or Astronomical
* __Season Type__ - Calendar or Special
* __Country Code__ - US
* __Language-Culture__ - en-US

###Season Formulas
* Date + CalendarType + SeasonType + Hemisphere = Season
* Date + CalendarType + SeasonType + CountryCode = Season

###Default Season Formulas
* Date + {CalendarType: Astronomical} + {SeasonType: Calendar} + {Hemisphere: Northern} = Season
* Date + {CalendarType: Astronomical} + {SeasonType: Calendar} + {CountryCode: US} = Season

###Estimated Season Formula
* Date + CalendarType + SeasonType + Language-Culture = Estimated Season

###Default Estimated Season Formula
* Date + {CalendarType: Astronomical} + {SeasonType: Calendar} + {Language-Culture: en-US} = Estimated Season

###How to derive the Hemisphere?
* __GPS Coordinate__ - Most mobile devices can derive this value
* __Country Code__ - Seasons.js will key off a set of known Southern Hemisphere countries
* __User Input__ - You could ask the client to input the hemisphere
* __Defaults__ - Seasons.js will default to Northern Hemisphere if no hemisphere is provided
* __Language-Culture__ - Seasons.js will *attempt* to key the hemisphere based on this parameter, results could vary

###Calendar Seasons
|                                   |
|:----------------------------------|
| **Traditional Seasons**           |
| Spring                            |
| Summer                            |
| Autumn                            |
| Winter                            |
|                                   |

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
*__Note__ special seasons isn't currently implemented in seasons.js, sorry.  We will work quickly to implement this feature in a future release.*


###Southern Hemisphere Countries

*The following countries are either entirely or mostly in the Southern Hemisphere per [Wikipedia](http://en.wikipedia.org/wiki/Southern_Hemisphere).*

*We will only key off of this list which contains countries in the Southern Hemisphere. If we don't find your country code we will assume the country is in the Northern Hemisphere.*

|                                   | Alpha-2 Code  | Alpha-3 Code  | Numeric Code  | ISO 3166-2    |
|:----------------------------------|:--------------|:--------------|:--------------|:--------------|
| **Africa**                                                                                        |
| Angola                            | AO            | AGO           | 024           | AF            |
| Botswana                          | BW            | BWA           | 072           | BW            |
| Burundi                           | BI            | BDI           | 108           | BI            |
| Comoros                           | KM            | COM           | 174           | KM            |
| Lesotho                           | LS            | LSO           | 426           | LS            |
| Madagascar                        | MG            | MDG           | 450           | MG            |
| Malawi                            | MW            | MWI           | 454           | MW            |
| Mauritius                         | MU            | MUS           | 480           | MU            |
| Mozambique                        | MZ            | MOZ           | 508           | MZ            |
| Namibia                           | NA            | NAM           | 516           | NA            |
| Rwanda                            | RW            | RWA           | 646           | RW            |
| Seychelles                        | SC            | SYC           | 690           | SC            |
| South Africa                      | ZA            | ZAF           | 710           | ZA            |
| Swaziland                         | SZ            | SWZ           | 748           | SZ            |
| Tanzania                          | TZ            | TZA           | 834           | TZ            |
| Zambia                            | ZM            | ZMB           | 894           | ZM            |
| Zimbabwe                          | ZW            | ZWE           | 716           | ZW            |
| Democratic Republic of the Congo  | CD            | COD           | 180           | CD            |
| Gabon                             | GA            | GAB           | 266           | GA            |
| Republic of the Congo             | CG            | COG           | 178           | CG            |
|                                                                                                   |
| **Asia**                                                                                          |
| East Timor                        | TL            | TLS           | 626           | TL            |
| Indonesia                         | ID            | IDN           | 360           | ID            |
|                                                                                                   |
| **Australia**                                                                                     |
| Australia                         | AU            | AUS           | 036           | AU            |
| Papua New Guinea                  | PG            | PNG           | 598           | PG            |
|                                                                                                   |
| **South America**                                                                                 |
| Argentina                         | AR            | ARG           | 032           | AR            |
| Bolivia                           | BO            | BOL           | 068           | BO            |
| Chile                             | CL            | CHL           | 152           | CL            |
| Paraguay                          | PY            | PRY           | 600           | PY            |
| Peru                              | PE            | PER           | 604           | PE            |
| Uruguay                           | UY            | URY           | 858           | UY            |
| Brazil                            | BR            | BRA           | 076           | BR            |
| Ecuador                           | EC            | ECU           | 218           | EC            |
|                                                                                                   | 
| **Pacific Ocean**                                                                                 |
| American Samoa                    | AS            | ASM           | 016           | AS            |
| Cook Islands                      | CK            | COK           | 184           | CK            |
| Easter Island                     |               |               |               |               |
| Fiji                              | FJ            | FJI           | 242           | FJ            |
| French Polynesia                  | PF            | PYF           | 258           | PF            |
| Galapagos Islands                 |               |               |               |               |
| Jarvis Island                     |               |               |               |               |
| Juan Fernandez Islands            |               |               |               |               |
| Nauru                             | NR            | NRU           | 520           | NR            |
| Territory of New Caledonia        | NC            | NCL           | 540           | NC            |
| New Zealand                       | NZ            | NZL           | 554           | NZ            |
| Niue                              | NU            | NIU           | 570           | NU            |
| Kermadec Islands                  |               |               |               |               |
| Pitcairn Islands                  | PN            | PCN           | 612           | PN            |
| Samoa                             | WS            | WSM           | 882           | WS            |
| Solomon Islands                   | SB            | SLB           | 090           | SB            |
| Swains Island                     |               |               |               |               |
| Tokelau                           | TK            | TKL           | 772           | TK            |
| Tonga                             | TO            | TON           | 776           | TO            |
| Tuvalu                            | TV            | TVU           | 798           | TV            |
| Vanuatu                           | VU            | VUT           | 548           | VU            |
| Wallis and Futuna                 | WF            | WLF           | 876           | WF            |
| **Atlantic Ocean**                                                                                |
| Falkland Islands                  | FK            | FLK           | 238           | FK            |
| Saint Helena                      | SH            | SHN           | 654           | SH            |
| Tristan da Cunha                  |               |               |               |               |
|                                                                                                   | 
| **Indian Ocean**                                                                                  |
| British Indian Ocean Territory    | IO            | IOT           | 086           | IO            |
| Mayotte                           | YT            | MYT           | 175           | YT            |
| Reunion                           | RE            | REU           | 638           | RE            |
|                                                                                                   | 
| **Southern Ocean**                                                                                |
| Antarctic islands                 | AQ            | ATA           | 010           | AQ            |
| Bouvet Island                     | BV            | BVT           | 074           | BV            |
| Kerguelen Islands                 |               |               |               |               |
| New Zealand SubAntarctic Islands  |               |               |               |               |
| Saint Paul and Amsterdam Island   |               |               |               |               |
| South Georgia & Sandwich Islands  | GS            | SGS           | 239           | GS            |
| South Orkney Islands              |               |               |               |               |
|                                                                                                   |

###Sources: 
- http://www.calendar-365.com/
- http://en.wikipedia.org/wiki/Season
- http://en.wikipedia.org/wiki/Southern_Hemisphere
- http://en.wikipedia.org/wiki/Country_code
- http://en.wikipedia.org/wiki/ISO_3166-1

###You may also be interested in:
- [Twilight.js] (https://github.com/erjjones/twilightjs) - A JavaScript library which derives the sun's position of the client - day, night, dawn/sunrise, dusk/sunset.
- [Earth.js] (https://github.com/erjjones/earthjs) - A JavaScript library which bundles [Seasons.js] (https://github.com/erjjones/seasonsjs) and [Twilight.js] (https://github.com/erjjones/twilightjs)

###License:
MIT License. Copyright 2012 Eric Jones. http://github.com/erjjones

Permission is hereby granted, free of charge, to any
person obtaining a copy of this software and associated
documentation files (the "Software"), to deal in the
Software without restriction, including without limitation
the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the
Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice
shall be included in all copies or substantial portions of
the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY
KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
