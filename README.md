#include <WiFi.h>
#include <esp_system.h>

void setup() {
  Serial.begin(115200);
  delay(2000);

  WiFi.mode(WIFI_STA);
  WiFi.begin();   // initialize WiFi hardware

  delay(1000);

  Serial.print("MAC Address: ");
  Serial.println(WiFi.macAddress());
}

void loop() {}
