Custom Components Integrations
  hacs
  openweathermaps
  smart irrigation
  zigbee2MQTT
  Mosquito Broker
  Visual Studio
  OneDrive

Themes
  cn-dark-mode
  dark_teal

Community Cards
  Bubble-card
  button-card
  lovelace-card-mod
  lovelace-mushroom
  weather-card
  weather-chart-card

Helpers
  {% set helpers = states | selectattr('entity_id', 'match', '^(input_|counter|number|schedule|timer|date|time|datetime|event|button)') | list %}
  {% for helper in helpers %}
  {{ helper.entity_id }}: {{ helper.state }} ({{ helper.attributes | to_json }})
  {% endfor %}
  
  event.backup_automatic_backup: 2025-12-02T18:25:58.141+00:00 ({"event_types":["completed","failed","in_progress"],"event_type":"completed","backup_stage":null,"failed_reason":null,"friendly_name":"Backup Automatic backup"})
  
  input_number.forecast_max_temperature: 28.6 ({"initial":null,"editable":true,"min":-20.0,"max":50.0,"step":0.1,"mode":"box","unit_of_measurement":"°C","friendly_name":"Forecast Max Temperature"})
  
  input_number.forecast_min_temperature: 10.0 ({"initial":null,"editable":true,"min":-20.0,"max":50.0,"step":0.1,"mode":"box","unit_of_measurement":"°C","friendly_name":"Forecast Min Temperature"})
  
  input_number.forecast_rain_amount: 2.58 ({"initial":null,"editable":true,"min":0.0,"max":100.0,"step":0.1,"mode":"slider","unit_of_measurement":"mm","friendly_name":"Forecast Rain Amount"})
  
  input_boolean.test_irrigation: off ({"editable":true,"friendly_name":"Test Irrigation"})
  
  input_text.forecast_data_storage: unknown ({"editable":true,"min":0,"max":100,"pattern":null,"mode":"text","friendly_name":"forecast_data_storage"})
  
  input_text.irrigation_status: Complete 08:55 PM ({"editable":true,"min":0,"max":100,"pattern":null,"mode":"text","friendly_name":"Irrigation Status"})
  
  input_text.weather_condition: unknown ({"editable":true,"min":0,"max":50,"pattern":null,"mode":"text","friendly_name":"Weather Condition"})
  
  button.slzb_06_core_restart: unknown ({"device_class":"restart","friendly_name":"SLZB-06 Core restart"})
  
  button.slzb_06_zigbee_restart: unknown ({"device_class":"restart","friendly_name":"SLZB-06 Zigbee restart"})
  
  button.zigbee2mqtt_bridge_restart: unavailable ({"restored":true,"device_class":"restart","friendly_name":"Restart","supported_features":0})


