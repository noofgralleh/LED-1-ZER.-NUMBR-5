# LED-1-ZER

## 💡 وصف المشروع

مشروع **LED-1-ZER** يوضح كيفية التحكم في إضاءة مصباح LED باستخدام لوحة تطوير مثل **Arduino**.  
يقوم المشروع بتشغيل وإيقاف (صفر) **LED رقم 1** المتصل باللوحة بطريقة برمجية.

## 🧰 المتطلبات

- لوحة تطوير (Arduino Uno أو مشابه)
- LED
- مقاومة 220 أوم
- أسلاك توصيل
- برنامج Arduino IDE

## ⚙️ التوصيل

- الطرف الموجب للـ LED → إلى المنفذ الرقمي رقم 7
- الطرف السالب → إلى المقاومة ثم إلى GND

## 💻 مثال على كود Arduino

```cpp
int ledPin = 7;

void setup() {
  pinMode(ledPin, OUTPUT);  // تعيين المنفذ كمخرج
}

void loop() {
  digitalWrite(ledPin, HIGH);  // تشغيل الـ LED
  delay(1000);                 // الانتظار لمدة ثانية
  digitalWrite(ledPin, LOW);   // إيقاف الـ LED (ZER)
  delay(1000);
}
