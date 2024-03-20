Giải thích code :

#define LED_PIN 2
void setup() {
  Serial.begin(115200); 
  pinMode(LED_PIN, OUTPUT); 
}

void loop() {
  digitalWrite(LED_PIN, HIGH); 
  Serial.println("LED is ON"); 
  delay(1000); //
  digitalWrite(LED_PIN, LOW); 
  Serial.println("LED is OFF"); 
  delay(1000); 
}


Đầu tiên ở phần setup():
 - Set serial để hiển thị ra mornitor
 - Chỉnh chế độ OUTPUT cho chân LED_PIN (GPIO 2)
Ở phần loop():
  - Gán tín hiệu digital HIGH (bật đèn)
  - In ra mornitor "LED is ON"
  - Đợi 1s
  - Gán tín hiệu digital LOW (tắt đèn)
  - In ra mornitor "LED is OFF"
  - Đợi 1s
    
