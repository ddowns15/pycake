# pycake Changelog

###v1.11.0
- November 29, 2017
- When ``CAKEApi.json_response=True``, functions will return a json object instead of a string

### v1.10.0
- November 9, 2017
- Better README including all functions documented below
- Added `CAKEApi.signup_advertiser()` function
- Added `CAKEApi.signup_affiliate()` function
- Added `CAKEApi.add_campaign_creative_exception()` function
- Added `CAKEApi.add_campaign_subid_exception()` function
- Added `CAKEApi.remove_campaign_creative_exception()` function
- Added `CAKEApi.remove_campaign_subid_exception()` function
- Fixed bug in ``CAKEApi.edit_affiliate()``. Some fields' default values were not skip values.
- Removed ``CAKEApi.edit_creative_files()``. While investigating a bug in this function I found a bug in the CAKE API that needs to be resolved before this fucntion can work properly. 

### v1.9.0
- October 27, 2017
- Added `CAKEApi.add_contact()`
- Added `CAKEApi.edit_caps()`
- Added `CAKEApi.edit_creative()`
- All `CAKEApi` methods now allow passing of additional keyword arguments (but they are ignored)
- Renamed `secure` argument to `use_https` when initializing a `CAKEApi` object
- Changed all error messaging to use the generic `Exception` type


### v1.8.0
- October 19, 2017
- Added `CAKEApi.add_creative()`
- Fixed incorrect date year in v1.7.0 entry of CHANGELOG.md

### v1.7.0
- September 25, 2017
- Added `CAKEApi.country_summary()` and `CAKEApi.lite_clicks_country_summary()`
- Added CHANGELOG.md
- Updated README.rst

### v1.6.1
- August 23, 2017
- Bug Fixes:
    - `CAKEApi.export_campaigns()` now requires at least one of the following arguments: `affiliate_id`, `offer_id`, `campaign_id`. This matches requirements in the underlying API.

### v1.6.0
- August 22, 2017
- Added `CAKEApi.affiliate_offer_feed()`

### v1.5.0
- August 22, 2017
- Added `CAKEApi.conversion_changes()`

### v1.4.0
- August 18, 2017
- Added `CAKEApi.export_offers()`

### v1.3.0
- July 27, 2017
- Updated version of underlying API call for `CAKEApi.conversions()`

### v1.2.1
- July 26, 2017
- Bug Fixes:
    - Resolved error caused by passing date/datetime objects as `start_date` and `end_date` arguments

### v1.2.0
- July 26, 2017
- Renamed `CAKEApi.daily_summary_export()` to `CAKEApi.daily_summary()`
- Added `CAKEApi.lite_clicks_daily_summary()`

### v1.1.0
- July 24, 2017
- Updated version of underlying API call for `CAKEApi.conversions()` and `CAKEApi.clicks()`

### v1.0.0
- July 14, 2017
- Initial release