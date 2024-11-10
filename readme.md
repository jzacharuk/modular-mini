# Slide (B103)

Assuming you are looking at the bottom, with 2 pins on the left, and 4 pins on the left.

Left Bottom to GND 
Right Bottom to 3V3
Right Second from Bottom to D1

There is an issue that the A0 values read only go from 9-1024, and the last 20% or so of the slide all return 1024.

void setup() {
  // Start the serial communication at 9600 baud rate
  Serial.begin(9600);
}

void loop() {
  // Read the analog value from pin A0 (range 0 to 1023)
  int sensorValue = analogRead(A0);
  
  // Print the value to the Serial Monitor
  Serial.println(sensorValue);
  
  // Add a small delay for readability
  delay(500);  // Delay in milliseconds (500ms)
}
