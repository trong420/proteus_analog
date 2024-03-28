<div align="center">

<h1>Proteus Projects</h1>
</div>

**Count up 6**

![image](https://github.com/trong420/proteus_analog/assets/90754954/6f1b5e97-0ff4-492b-a34e-d151ec2a609e)

**Count up 9**


![image](https://github.com/trong420/proteus_analog/assets/90754954/b1e5bec3-f166-49db-8fcb-10ca013c5064)


**Count down 7**

![image](https://github.com/trong420/proteus_analog/assets/90754954/6c9751d1-e0b9-4dbe-bc10-af4b548dfce4)


**Count down 12**

![image](https://github.com/trong420/proteus_analog/assets/90754954/f19c573c-5755-4176-bbd9-4eba25741417)



**Count 1-10**

![image](https://github.com/trong420/proteus_analog/assets/90754954/507d3cc3-4a99-43a5-a082-b1aac57b8bd3)


**Clock with IC555**

![image](https://github.com/trong420/proteus_analog/assets/90754954/99454bdb-be1d-452f-a010-36d633765e7f)


**Shift left**

![image](https://github.com/trong420/proteus_analog/assets/90754954/b2cce5a7-fbac-4727-8c10-49f31810ceb2)


**Shift right**


![image](https://github.com/trong420/proteus_analog/assets/90754954/0ff8f711-3e92-4434-9954-17163a7c1d82)


**Ring counter**

![image](https://github.com/trong420/proteus_analog/assets/90754954/c1a1920b-ac65-44fe-b344-877faa523e1d)

**Text Scrolling Circuit**

- Code:

```c
#include <LiquidCrystal.h>

LiquidCrystal lcd(12, 11, 5, 4, 3, 2);
int Li = 16;
int Lii = 0;
int Ri = -1;
int Rii = -1;
void setup() {
  lcd.begin(16, 2);
}
void loop() {
  lcd.setCursor(0, 0);
  lcd.print(" 19200536 ");
  lcd.setCursor(0, 1);
  lcd.print(Scroll_LCD_Left("FETEL - HCMUS"));
  delay(80);
}

String Scroll_LCD_Left(String StrDisplay) {
  String result;
  String StrProcess = " " + StrDisplay + " ";
  result = StrProcess.substring(Li, Lii);
  Li++;
  Lii++;
  if (Li > StrProcess.length()) {
    Li = 16;
    Lii = 0;
  }
  return result;
}
```
  
![image](https://github.com/trong420/proteus_analog/assets/90754954/da13f494-6be7-4df3-b9eb-e06453202026)


**Triangular Wave Oscillator Circuit**

![image](https://github.com/trong420/proteus_analog/assets/90754954/9df6f143-6ad8-4135-9451-ce7066cd38df)


**Bandpass Filter**

![image](https://github.com/trong420/proteus_analog/assets/90754954/7ba7e561-46bb-4e08-af7f-441116accef2)


**Inverter Trigger Schmitt**

![image](https://github.com/trong420/proteus_analog/assets/90754954/8a67568b-7e75-4b6b-9639-896d79c9ae24)

**Precision Rectifier Circuit**

![image](https://github.com/trong420/proteus_analog/assets/90754954/930ee15d-3a12-41ee-b646-80e25f32eb4f)


**Flash ADC 8 Bit**

![image](https://github.com/trong420/proteus_analog/assets/90754954/5c263cd2-6bbf-4818-b6b9-ce67f42b9255)
