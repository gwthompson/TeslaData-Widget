# Overview of the fields in that are consumed by the widget.

## Required
* usable_battery_level : the actual usable amount (0-100), this is used when the battery is cold
* charge_limit_soc : the charge limit you have configured for the car (0-100)

Although, it's a good idea to include all of the following fields, the widget will still render what it can when you include any of the following fields.

## Optional
* response : should be null unless there is an error
* Date : the last contact with the vehicle (This can be almost any date format, but should include date and time, TelsaFi uses UTC style YYYY-MM-DD HH:MM:SS)
* battery_level : the current battery value (0-100)
* carState : the current state of the car (Sleeping, Charging, Driving, Idle)
* sentry_mode : is sentry mode on (0 or 1)
* display_name : the name of the car (as defined by the user)
* locked : are the doors locked (0 or 1)
* is_climate_on : is the car's climate system on (0 or 1)
* inside_temp : the inside temperature of the car in C
* driver_temp_setting : the set temp for the climate control in C
* temperature : if we should display F or C temperatures
* inside_tempF : the inside temperature of the car in F (only used if temperature == F)
* driver_temp_settingF : the set temp for the climate control in F (only used if temperature == F)
* measure : if the range/distance measurements are in km or m
* battery_range : the range of the car (as calculated by the car)
* est_battery_range : the range of the car (as calculated by the logging service)
* time_to_full_charge : how long until the car is fully charged
* fast_charger_type : what kind of charger is attached. Should be "<invalid>" if the car is not connected to a charger (the widget only checks to see if it's attached, so the actual type is unimportant).
* latitude : the latitude location of the car
* longitude : the longitude location of the car
