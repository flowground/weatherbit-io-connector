# ![LOGO](logo.png) Weatherbit.io - Swagger UI Weather API documentation **flow**ground Connector

## Description

A generated **flow**ground connector for the Weatherbit.io - Swagger UI Weather API documentation API (version 2.0.0).

Generated from: https://api.apis.guru/v2/specs/weatherbit.io/2.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:44:52+03:00

## API Description

This is the documentation for the Weatherbit Weather API.  The base URL for the API is [http://api.weatherbit.io/v2.0/](http://api.weatherbit.io/v2.0/) or [https://api.weatherbit.io/v2.0/](http://api.weatherbit.io/v2.0/). Below is the Swagger UI documentation for the API. All API requests require the `key` parameter.        An Example for a 5 day forecast for London, UK would be `http://api.weatherbit.io/v2.0/forecast/3hourly?city=London`&`country=UK`. See our [Weather API description page](https://www.weatherbit.io/api) for additional documentation.

## Authorization

This API does not require authorization.

## Actions

### Returns severe weather alerts issued by meteorological agencies - Given a lat/lon.

> Returns severe weather alerts issued by meteorological agencies - given a lat, and a lon.

*Tags:* `Alerts`

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `callback` - _optional_ - Wraps return in jsonp callback - Example - callback=func
* `key` - _required_ - Your registered API key.

### Download pre-generated bulk datasets

> **(Advanceed/Enterprise plans only)** Downloads bulk data files - OPTIONS: ( current.json.gz - Current observations for cities > 1000 population). Units are Metric (Celcius, m/s, etc).

*Tags:* `Bulk Downloads`

#### Input Parameters
* `file` - _required_ - Filename (ie. current.json.gz)
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given City and/or State, Country.

> Returns Historical Observations - Given a city in the format of City,ST or City. The state, and country parameters can be provided to make the search more accurate.

*Tags:* `(Bulk) Daily Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `city` - _required_ - City search.. Example - &city=Raleigh,NC or &city=Berlin,DE or city=Paris&country=FR
* `state` - _optional_ - Full name of state.
* `country` - _required_ - Country Code (2 letter).
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given a City ID

> Returns Historical Observations - Given a City ID.

*Tags:* `(Bulk) Daily Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `city_id` - _required_ - City ID. Example: 4487042
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given IP Address, or auto.

> Returns Historical Observations - Given IP Address, or auto.

*Tags:* `(Bulk) Daily Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `ip` - _required_ - IP Address, or auto. Example: ip=auto
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given a lat/lon.

> Returns Historical Observations - Given a lat, and lon.

*Tags:* `(Bulk) Daily Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given a Postal Code

> Returns Historical Observations - Given a Postal Code.

*Tags:* `(Bulk) Daily Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `postal_code` - _required_ - Postal Code. Example: 28546
* `country` - _optional_ - Country Code (2 letter).
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given a station ID.

> Returns Historical Observations - Given a station ID.

*Tags:* `(Bulk) Daily Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `station` - _required_ - Station ID.
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given City and/or State, Country. (1 Year/call limit)

> Returns Historical Observations - Given a city in the format of City,ST or City. The state, and country parameters can be provided to make the search more accurate.

*Tags:* `(Bulk) Hourly Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `city` - _required_ - City search.. Example - &city=Raleigh,NC or &city=Berlin,DE or city=Paris&country=FR
* `state` - _optional_ - Full name of state.
* `country` - _required_ - Country Code (2 letter).
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given a City ID. (1 Year/call limit)

> Returns Historical Observations - Given a City ID.

*Tags:* `(Bulk) Hourly Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `city_id` - _required_ - City ID. Example: 4487042
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given IP Address, or auto. (1 Year/call limit)

> Returns Historical Observations - Given IP Address, or auto.

*Tags:* `(Bulk) Hourly Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `ip` - _required_ - IP Address, or auto. Example: ip=auto
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given a lat/lon. (1 Year/call limit)

> Returns Historical Observations - Given a lat, and lon.

*Tags:* `(Bulk) Hourly Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given a Postal Code. (1 Year/call limit)

> Returns Historical Observations - Given a Postal Code.

*Tags:* `(Bulk) Hourly Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `postal_code` - _required_ - Postal Code. Example: 28546
* `country` - _optional_ - Country Code (2 letter).
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### [Enterprise Plan Only] Returns Historical Observations - Given a station ID. (1 Year/call limit)

> Returns Historical Observations - Given a station ID.

*Tags:* `(Bulk) Hourly Historical Weather Data (Enterprise Plans)`

#### Input Parameters
* `station` - _required_ - Station ID.
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns a group of observations given a list of cities

> Returns a group of Current Observations - Given a list of City IDs.

*Tags:* `Current Weather Data`

#### Input Parameters
* `cities` - _required_ - Comma separated list of City ID's. Example: 4487042, 4494942, 4504871
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `marine` - _optional_ - Marine stations only (buoys, oil platforms, etc)
    Possible values: t.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback - Example - callback=func
* `key` - _required_ - Your registered API key.

### Returns a Current Observation - Given City and/or State, Country.

> Returns a Current Observation - Given a city in the format of City,ST or City. The state, and country parameters can be provided to make the search more accurate.

*Tags:* `Current Weather Data`

#### Input Parameters
* `city` - _required_ - City search.. Example - &city=Raleigh,NC or &city=Berlin,DE or city=Paris&country=FR
* `state` - _optional_ - Full name of state.
* `country` - _required_ - Country Code (2 letter).
* `marine` - _optional_ - Marine stations only (buoys, oil platforms, etc)
    Possible values: t.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback - Example - callback=func
* `key` - _required_ - Your registered API key.

### Returns a current observation by city id.

> Returns current weather observation - Given a City ID.

*Tags:* `Current Weather Data`

#### Input Parameters
* `city_id` - _required_ - City ID. Example: 4487042
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `marine` - _optional_ - Marine stations only (buoys, oil platforms, etc)
    Possible values: t.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback - Example - callback=func
* `key` - _required_ - Your registered API key.

### Returns a Current Observation - Given an IP address, or auto.

*Tags:* `Current Weather Data`

#### Input Parameters
* `ip` - _required_ - IP Address, or auto. Example: ip=auto
* `marine` - _optional_ - Marine stations only (buoys, oil platforms, etc)
    Possible values: t.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback - Example - callback=func
* `key` - _required_ - Your registered API key.

### Returns a Current Observation - Given a lat/lon.

> Returns a Current Observation - given a lat, and a lon.

*Tags:* `Current Weather Data`

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `marine` - _optional_ - Marine stations only (buoys, oil platforms, etc)
    Possible values: t.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback - Example - callback=func
* `key` - _required_ - Your registered API key.

### Returns a current observation by postal code.

> Returns current weather observation - Given a Postal Code.

*Tags:* `Current Weather Data`

#### Input Parameters
* `postal_code` - _required_ - Postal Code. Example: 28546
* `country` - _optional_ - Country Code (2 letter).
* `marine` - _optional_ - Marine stations only (buoys, oil platforms, etc)
    Possible values: t.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback - Example - callback=func
* `key` - _required_ - Your registered API key.

### Returns a Current Observation. - Given a station ID.

> Returns a Current Observation - Given a station ID.

*Tags:* `Current Weather Data`

#### Input Parameters
* `station` - _required_ - Station Call ID.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns a group of observations given a list of stations

> Returns a group of Current Observations - Given a list of Station Call IDs.

*Tags:* `Current Weather Data`

#### Input Parameters
* `stations` - _required_ - Comma separated list of Station Call ID's. Example: KRDU,KBFI,KVNY
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns a 3-hourly forecast - Given City and/or State, Country.

> Returns a 3-hourly forecast, where each point represents a three hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH". Time is UTC.

*Tags:* `5 day / 3 hour Forecast`

#### Input Parameters
* `city` - _required_ - City search.. Example - &city=Raleigh,NC or &city=Berlin,DE or city=Paris&country=FR
* `state` - _optional_ - Full name of state.
* `country` - _required_ - Country Code (2 letter).
* `days` - _optional_ - Number of days to return. Default 5.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example - callback=func
* `key` - _required_ - Your registered API key.

### Returns a 3-hourly forecast - Given a City ID.

> Returns a 3-hourly forecast, where each point represents a three hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH". Time is UTC.

*Tags:* `5 day / 3 hour Forecast`

#### Input Parameters
* `city_id` - _required_ - City ID. Example: 4487042
* `days` - _optional_ - Number of days to return. Default 5.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns a 3hourly forecast - Given an IP Address, or ip=auto for automatic IP lookup.

> Returns a 3-hourly forecast, where each point represents a three hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH". Time is UTC.

*Tags:* `5 day / 3 hour Forecast`

#### Input Parameters
* `ip` - _required_ - IP address, or auto. Example: ip=auto
* `days` - _optional_ - Number of days to return. Default 16.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns a 3-hourly forecast - Given a lat/lon.

> Returns a 3-hourly forecast, where each point represents a three hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH". Time is UTC.

*Tags:* `5 day / 3 hour Forecast`

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `days` - _optional_ - Number of days to return. Default 5.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example - callback=func
* `key` - _required_ - Your registered API key.

### Returns a 3-hourly forecast - Given a Postal Code.

> Returns a 3-hourly forecast, where each point represents a three hour period. Every point has a datetime string in the format "YYYY-MM-DD:HH". Time is UTC.

*Tags:* `5 day / 3 hour Forecast`

#### Input Parameters
* `postal_code` - _required_ - Postal Code. Example: 28546
* `country` - _optional_ - Country Code (2 letter).
* `days` - _optional_ - Number of days to return. Default 5.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns a daily forecast - Given City and/or State, Country.

> Returns a daily forecast, where each point represents one day (24hr) period. Every point has a datetime string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at 23:59 UTC. Accepts a city in the format of City,ST or City. The state, and country parameters can be provided to make the search more accurate.

*Tags:* `16 day / daily Forecast`

#### Input Parameters
* `city` - _required_ - City search.. Example - &city=Raleigh,NC or &city=Berlin,DE or city=Paris&country=FR
* `state` - _optional_ - Full name of state.
* `country` - _required_ - Country Code (2 letter).
* `days` - _optional_ - Number of days to return. Default 16.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example - callback=func
* `key` - _required_ - Your registered API key.

### Returns a daily forecast - Given a City ID.

> Returns a daily forecast, where each point represents one day (24hr) period. Every point has a datetime string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at 23:59 UTC.

*Tags:* `16 day / daily Forecast`

#### Input Parameters
* `city_id` - _required_ - City ID. Example: 4487042
* `days` - _optional_ - Number of days to return. Default 16.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns a daily forecast - Given an IP Address, or ip=auto for automatic IP lookup.

> Returns a daily forecast, where each point represents one day (24hr) period. Every point has a datetime string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at 23:59 UTC.

*Tags:* `16 day / daily Forecast`

#### Input Parameters
* `ip` - _required_ - IP address, or auto. Example: ip=auto
* `days` - _optional_ - Number of days to return. Default 16.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns a daily forecast - Given Lat/Lon.

> Returns a daily forecast, where each point represents one day (24hr) period. Every point has a datetime string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at 23:59 UTC.

*Tags:* `16 day / daily Forecast`

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `days` - _optional_ - Number of days to return. Default 16.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns a daily forecast - Given a Postal Code.

> Returns a daily forecast, where each point represents one day (24hr) period. Every point has a datetime string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at 23:59 UTC.

*Tags:* `16 day / daily Forecast`

#### Input Parameters
* `postal_code` - _required_ - Postal Code. Example: 28546
* `country` - _optional_ - Country Code (2 letter).
* `days` - _optional_ - Number of days to return. Default 16.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Energy Forecast API response  - Given a single lat/lon.

> Retrieve an 8 day forecast relevant to te Energy Sector (degree days, solar radiation, precipitation, wind).

*Tags:* `Forecast Degree Day API` `Forecast Solar Irradiance API`

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `threshold` - _optional_ - Temperature threshold to use to calculate degree days (default 18 C) 
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns an 48 hour (hourly forecast) - Given City and/or State, Country.

> Returns an hourly forecast, where each point represents a one hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH". Time is UTC. Accepts a city in the format of City,ST or City. The state, and country parameters can be provided to make the search more accurate.

*Tags:* `48 hour / hourly Forecast`

#### Input Parameters
* `city` - _required_ - City search.. Example - &city=Raleigh,NC or &city=Berlin,DE or city=Paris&country=FR
* `state` - _optional_ - Full name of state.
* `country` - _required_ - Country Code (2 letter).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `hours` - _optional_ - Number of hours to return.
* `key` - _required_ - Your registered API key.

### Returns a 48 hour (hourly) forecast - Given a City ID.

> Returns an hourly forecast, where each point represents a one hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH". Time is UTC.

*Tags:* `48 hour / hourly Forecast`

#### Input Parameters
* `city_id` - _required_ - City ID. Example: 4487042
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example - callback=func
* `hours` - _optional_ - Number of hours to return.
* `key` - _required_ - Your registered API key.

### Returns a hourly forecast - Given an IP Address, or ip=auto for automatic IP lookup.

> Returns an hourly forecast, where each point represents a one hour period. Every point has a datetime string in the format "YYYY-MM-DD:HH". Time is UTC.

*Tags:* `48 hour / hourly Forecast`

#### Input Parameters
* `ip` - _required_ - IP address, or auto. Example: ip=auto
* `days` - _optional_ - Number of days to return. Default 16.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `hours` - _optional_ - Number of hours to return.
* `key` - _required_ - Your registered API key.

### Returns 48 hour (hourly) forecast - Given a lat/lon.

> Returns an hourly forecast, where each point represents a one hour period. Every point has a datetime string in the format "YYYY-MM-DD:HH". Time is UTC.

*Tags:* `48 hour / hourly Forecast`

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example - callback=func
* `key` - _required_ - Your registered API key.
* `hours` - _optional_ - Number of hours to return.

### Returns a 48 hour (hourly) forecast - Given a Postal Code.

> Returns an hourly forecast, where each point represents a one hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH". Time is UTC.

*Tags:* `48 hour / hourly Forecast`

#### Input Parameters
* `postal_code` - _required_ - Postal Code. Example: 28546
* `country` - _optional_ - Country Code (2 letter).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example - callback=func
* `hours` - _optional_ - Number of hours to return.
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given City and/or State, Country.

> Returns Historical Observations - Given a city in the format of City,ST or City. The state, and country parameters can be provided to make the search more accurate. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Daily Historical Weather Data`

#### Input Parameters
* `city` - _required_ - City search.. Example - &city=Raleigh,NC or &city=Berlin,DE or city=Paris&country=FR
* `state` - _optional_ - Full name of state.
* `country` - _required_ - Country Code (2 letter).
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given a City ID

> Returns Historical Observations - Given a City ID. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Daily Historical Weather Data`

#### Input Parameters
* `city_id` - _required_ - City ID. Example: 4487042
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given IP Address, or auto.

> Returns Historical Observations - Given IP Address, or auto. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Daily Historical Weather Data`

#### Input Parameters
* `ip` - _required_ - IP Address, or auto. Example: ip=auto
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given a lat/lon.

> Returns Historical Observations - Given a lat, and lon. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Daily Historical Weather Data`

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given a Postal Code

> Returns Historical Observations - Given a Postal Code. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Daily Historical Weather Data`

#### Input Parameters
* `postal_code` - _required_ - Postal Code. Example: 28546
* `country` - _optional_ - Country Code (2 letter).
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given a station ID.

> Returns Historical Observations - Given a station ID. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Daily Historical Weather Data`

#### Input Parameters
* `station` - _required_ - Station ID.
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns multiple locations given a bounding box.

> Returns aggregate energy specific historical weather fields, over a specified time period. Supply a bounding box ex: lat1=40&lon1=-78&lat2=38&lon2=-80. This API will return UP TO 150 stations, aggregated by the specified time period start_date to end_date.

*Tags:* `Historical Degree Day API` `Historical Solar Irradiance API` `Historical Weather Energy API`

#### Input Parameters
* `lat1` - _required_ - Latitude of upper left corner.
* `lon1` - _required_ - Longitude of upper left corner.
* `lat2` - _required_ - Latitude of lower right corner.
* `lon2` - _required_ - Longitude of lower right corner.
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `threshold` - _optional_ - Temperature threshold to use to calculate degree days (default 18 C) 
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Energy API response  - Given a single lat/lon.

> Returns aggregate energy specific historical weather fields, over a specified time period.

*Tags:* `Historical Degree Day API` `Historical Solar Irradiance API` `Historical Weather Energy API`

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `tp` - _optional_ - Time period to aggregate by (daily, monthly)
    Possible values: daily, monthly.
* `threshold` - _optional_ - Temperature threshold to use to calculate degree days (default 18 C) 
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given City and/or State, Country.

> Returns Historical Observations - Given a city in the format of City,ST or City. The state, and country parameters can be provided to make the search more accurate. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Hourly Historical Weather Data`

#### Input Parameters
* `city` - _required_ - City search. Example - &city=Raleigh,NC or &city=Berlin,DE or city=Paris&country=FR
* `state` - _optional_ - Full name of state.
* `country` - _required_ - Country Code (2 letter).
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `tz` - _optional_ - Assume utc (default) or local time for start_date, end_date
    Possible values: local, utc.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given a City ID

> Returns Historical Observations - Given a City ID. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Hourly Historical Weather Data`

#### Input Parameters
* `city_id` - _required_ - City ID. Example: 4487042
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `tz` - _optional_ - Assume utc (default) or local time for start_date, end_date
    Possible values: local, utc.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given IP Address, or auto.

> Returns Historical Observations - Given IP Address, or auto. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Hourly Historical Weather Data`

#### Input Parameters
* `ip` - _required_ - IP Address, or auto. Example: ip=auto
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `tz` - _optional_ - Assume utc (default) or local time for start_date, end_date
    Possible values: local, utc.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given a lat/lon.

> Returns Historical Observations - Given a lat, and lon. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Hourly Historical Weather Data`

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `tz` - _optional_ - Assume utc (default) or local time for start_date, end_date
    Possible values: local, utc.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given a Postal Code

> Returns Historical Observations - Given a Postal Code. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Hourly Historical Weather Data`

#### Input Parameters
* `postal_code` - _required_ - Postal Code. Example: 28546
* `country` - _optional_ - Country Code (2 letter).
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `tz` - _optional_ - Assume utc (default) or local time for start_date, end_date
    Possible values: local, utc.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns Historical Observations - Given a station ID.

> Returns Historical Observations - Given a station ID. **(LIMIT 1 day for Free plan. LIMIT 7 days for Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**

*Tags:* `Hourly Historical Weather Data`

#### Input Parameters
* `station` - _required_ - Station ID.
* `start_date` - _required_ - Start Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `end_date` - _required_ - End Date (YYYY-MM-DD or YYYY-MM-DD:HH).
* `units` - _optional_ - Convert to units. Default Metric See <a target='blank' href='/api/requests'>units field description</a>
    Possible values: S, I.
* `lang` - _optional_ - Language (Default: English) See <a target='blank' href='/api/requests'>language field description</a>
    Possible values: ar, az, be, bg, bs, ca, cs, de, fi, fr, el, es, et, hr, hu, id, it, is, kw, nb, nl, pl, pt, ro, ru, sk, sl, sr, sv, tr, uk, zh, zh-tw.
* `tz` - _optional_ - Assume utc (default) or local time for start_date, end_date
    Possible values: local, utc.
* `callback` - _optional_ - Wraps return in jsonp callback. Example: callback=func
* `key` - _required_ - Your registered API key.

### Returns an Geolocation object.

> Returns a geolocation object. Given an IP address. If no IP supplied, will use request IP address.

*Tags:* `IP Geolocation API`

#### Input Parameters
* `ip` - _required_ - IP address
* `callback` - _optional_ - Wraps return in jsonp callback
* `exclude` - _optional_ - exclude=all => return IP address only
* `format` - _optional_ - &format=none => return IP address as string
* `key` - _required_ - Your registered API key.

## License

**flow**ground :- Telekom iPaaS / weatherbit-io-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
