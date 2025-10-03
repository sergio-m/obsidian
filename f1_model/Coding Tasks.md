cd

 From list of years
	- [ ] Populate seasons (year, circuit_id)
	- [ ] Populate circuits (circuit_id, name, locality, country, lat, long, url)
	- [ ] Add type to fact_season (R, Q)
	- [ ] Build Session object
	- [ ] From fastf1.get_session(2024, 19, "R") update fact_season
		- [ ] official_name
		- [ ] start datetime
		- [ ] end datetime
		- [ ] type
		- [ ] Update DB using update_season_qry(year, event_number, circuit_id, official_name, start, end, type)
	- [ ] Session has
		- [ ] driver_info
		- [ ] session_status_data
		- [ ] lap_count
		- [ ] track_status_data
		- [ ] \_extended_timeing_data
		- [ ] timing_app_data
		- [ ] car_data
		- [ ] position_data
		- [ ] weather_data
		- [ ] race_control_messages