- colordiff -Naur
- ## Comandos utiles de emqx
	- Broker de MQTT escrito en earlang. [[emqx]]
- ## Systemd service
	- ```ini
	  [Unit]
	  Description=ROT13 demo service
	  After=network.target
	  StartLimitIntervalSec=0
	  [Service]
	  Type=simple
	  Restart=always
	  RestartSec=1
	  User=centos
	  ExecStart=/usr/bin/env php /path/to/server.php
	  [Install]
	  WantedBy=multi-user.target
	  ```
- ## Format spiffs partition on ESP-IDF
	- ```c
	  esp_spiffs_format("partition_label")
	  ```
- ## Set time manually in C (ESP-IDF)
	- ```c
	  struct tm tm;
	  tm.tm_year = (Runtime.year + 2000) - 1900;
	  tm.tm_mon = Runtime.month - 1;
	  tm.tm_mday = Runtime.day;
	  tm.tm_hour = Runtime.hour;
	  tm.tm_min = Runtime.minute;
	  tm.tm_sec = Runtime.second;
	  time_t t = mktime(&tm);
	  ESP_LOGI(TAG, "Setting System Time: %s", asctime(&tm));
	  struct timeval now = { .tv_sec = 0 };
	  settimeofday(&now, NULL);
	  ```
- JSON Macros
	- ```c
	  #define CREATE_JSON(buff,len,key,val,type)         snprintf(buff, len,"{\"%s\":" type "}",key,val)
	  #define CREATE_JSON_DOUBLE(buff,len,key,val)       CREATE_JSON(buff,len,key,val,"%f")
	  #define CREATE_JSON_INT(buff,len,key,val)          CREATE_JSON(buff,len,key,val,"%d")
	  #define CREATE_JSON_STR(buff,len,key,val)          snprintf(buff, len,"{\"%s\":\"%s\"}",key,val)
	  #define CREATE_JSON_NULL(buff,len,key)             snprintf(buff, len,"{\"%s\":null}",key)
	  ```