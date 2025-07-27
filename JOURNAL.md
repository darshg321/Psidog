# Quadruped Dog
Total Hours (so far): 4 hours
## july 26th, 2025
i was inspired to make this project from this article i saw: 
https://www.cnx-software.com/2024/08/08/mechdog-ai-robot-dog-features-esp32-s3-controller-supports-scratch-python-and-arduino-programming/ 

i've also always thought both boston dynamic's robot dog and MIT's mini cheetah were very cool, and i now am confident i finally have the knowledge to create a similar quadruped robot dog thanks to both designing my own drone and hackclub's undercity hackathon

this dog will be much smaller than boston dynamic's dog, currently estimating somewhere around 250mm * 150mm * 150mm, and weigh maybe around 500g

## goals/features:
- 8DOF
- traverses rough terrain (dirt)
- 30 minute battery life
- AI facial detection
- self balancing
- bluetooth controller or app driving
- autonomous pathing
- line following
- touch, temperature, lighting sensing
- voice control
- cliff detection
- obstacle detection
- USB-C self charging

more complicated features id like to implement if possible
- LIDAR terrain mapping
- walk up small stairs

tasks it should be able to accomplish:
- walk with me to the local path while i control with an xbox controller (~30 mins)
- deliver a small object to a specific person with facial detection
- voice command it to line follow to a charger and charge
- follow an autonomous path to another room in my apartment from mine
- map the terrain and send it back to my computer
- not fall off a table

# Parts

rough parts i will need
- microcontroller
- (opt): coprocessor for LIDAR and AI
- accelerometer, gyroscope
- camera
- USB-C PD
- ultrasonic sensor
- microphone and speaker
- touch sensor
- light sensor
- battery
- LIDAR
- servo
- servo driver
- voltage regulator
- OLED screen
- (opt): leg encoders

### microcontroller
ill be using a variant of the esp32, as its a very well established microcontroller and best suited for a mini dog like this one

based on the variants, theres a few choices:

- ESP32-S3-WROOM-1-N16R8
- ESP32-WROVER-IE-N16R8
- ESP32-S3-WROOM-2-N32R8V

theres also ESP32-S3-WROOM-2-N32R16V, which is just more psram and therefore better, but it's a new product and unavailable right now so i wont design this project around it

based on the variants, i'll be going with the wroom-2-N32R8V
it has 32mb flash, 8mb PSRAM, BLE 5.0, UART, camera support, and while it is discontinued, the benefits of it outweigh this con

while looking for variants i also found this cool site to find parts: https://octopart.com/

+4 hours
### servos



# PCB

