# First-Task-RobotArm

#include <Servo.h>

int i = 0;

int mov = 0;

int j = 0;

Servo servo_9;

void setup()
{
  servo_9.attach(9, 500, 2500);

}

void loop()
{
  mov = 0;
  for (mov = 1; mov <= 89; mov += 1) {
    servo_9.write(mov);
    delay(20); // Wait for 20 millisecond(s)
  }

  for (j = 89; j >= 1; j -= 1) {
    servo_9.write(mov);
  }
}


![First](https://user-images.githubusercontent.com/86917834/124694423-e70bf980-dee9-11eb-93a2-40c7f6e3b4d3.jpeg)
