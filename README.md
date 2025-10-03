# LED-1-ZER.
const int ledPin = 13;     // رقم البن المتصل بـ LED
const int buttonPin = 2;   // رقم البن المتصل بالزر
int buttonState = 0;       // لتخزين حالة الزر

void setup() {
  pinMode(ledPin, OUTPUT);       // ضبط البن كـ مخرج
  pinMode(buttonPin, INPUT);     // ضبط البن كـ مدخل
}

void loop() {
  buttonState = digitalRead(buttonPin);  // قراءة حالة الزر

  if (buttonState == HIGH) {
    digitalWrite(ledPin, HIGH);   // تشغيل الـ LED
  } else {
    digitalWrite(ledPin, LOW);    // إطفاء الـ LED
  }
}
