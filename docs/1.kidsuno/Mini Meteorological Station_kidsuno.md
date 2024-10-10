# Mini Meteorological Station for kidsuno

## 1. Code

[DOWNLOAD](../Code.zip)

Download and unzip these files. Here all codes are in folder **1.Code_kidsuno**.

For convenience, <span style="color: rgb(2550, 10, 50);">we move the codes into: **D:\Code\1.Code_kidsuno**.</span> You can also choose to move it into any disks at will. 

---

## 2. Development Environment Configuration

### 2.1 KidsBlock Download

![2101](media/2101.png)

1. [KidsBlock Download](https://wiki.kidsbits.cc/projects/KidsBlock/en/latest/download/)
2. Installation
	- [Windows System](https://wiki.kidsbits.cc/projects/KidsBlock/en/latest/Windows/)
	- [MacOS System](https://wiki.kidsbits.cc/projects/KidsBlock/en/latest/MacOS/)
3. [Driver Installation](https://wiki.kidsbits.cc/projects/KidsBlock/en/latest/driver/)

---

### 2.2 KidsBlock Tutorial

1. Make sure the board is connected to computer. Open KidsBlock and choose a device.

![2201](media/2201.png)

Choose **kidsuno**.

![2202](media/2202.png)

Click **Connect**.

![2203](media/2203.png)

**Go to Editor**.

![2204](media/2204.png)

Click ![2216](media/2216.png) to switch to upload mode.

![2215](media/2215.png)

![2217](media/2217.png)

![line1](media/line1.png)

2. Build code blocks and upload.

**Method ①**: Directly drag blocks to the editing area.

![2207](media/2207.png)

After building your blocks, save it to your computer: **File --> Save to your computer**

![2209](media/2209.png)

Click ![2210](media/2210.png) to upload the code.

![line4](media/line4.png)

**Method ②**: Load code from your computer.

Download code in **1. Code** to your computer. For convenience, here we save it to D:\Code\1.Code_kidsuno.

**File --> Load from your computer** and choose code to open.

![2209](media/2209.png)

After loading code, connect to the corresponding port.

![2211](media/2211.png)

![2203](media/2203.png)

After that, click ![2210](media/2210.png)to upload code.

![line1](media/line1.png)

**Main Interface**

![2205](media/2205.png)

![2206](media/2206.png)

---

## 3. Modules

<span style="color: rgb(2550, 10, 50);">Please move the codes to a convenient path as your needs, for instance, path: **D:\Code\1.Code_kidsuno**.</span>

### kidsuno Ports View

During experiments, <span style="color: rgb(2550, 10, 50);">modules can only be connected to ports in the same color.</span>

![KD2075](media/KD2075.png)

### 3.1 White LED Module

![1top](media/1top.png)

![KD2078](media/KD2078.png)

**LED (Light-Emitting Diode)**

LED is a commonly used light emitting device that converts electrical energy into light energy. Usually, it is used as an indicator in circuits and instruments, or as part of texts or numeric display.

It generally includes gallium(Ga), arsenic(As), phosphorus(P), nitrogen(N) and so on. 

|     LED components      | Emitting light colors |
| :---------------------: | :-------------------: |
| gallium arsenide diode  |          red          |
| gallium phosphide diode |         green         |
|  silicon carbide diode  |        yellow         |
|  gallium nitride diode  |         blue          |

![1bottom](media/1bottom.png)

#### Parameters

![2top](media/2top.png)

Operating voltage: DC 3.3 ~ 5 V

Operating current: 1.5 mA (Peak: 2.3mA)

Maximum power: 0.07 W

Control signal: digital signal

Dimensions: 24 x 48 x 18 mm (without housing)

Positioning holes: diameter of 4.8 mm

Interface: telephone socket

![2bottom](media/2bottom.png)

#### Principle

![3top](media/3top.png)

Modules with blue housing are digital ones, so we should connect to digital io pins of the mainboard (ports with blue).

![uno-blue](media/uno-blue.png)

In this experiment, we connect the white LED module to port 1. According to the board ports view, the digital io pin at port 1 is D5.

When we set the pin to high(1), the LED lights up in white; if we set to low(0), it will be off.

![3bottom](media/3bottom.png)

#### Wiring Diagram

![3101](media/3101.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **3.1Light_on.sb3** file.

![3102](media/3102.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Code Blocks**

|            Blocks             |          Code block           |
| :---------------------------: | :---------------------------: |
|  ![Events](media/Events.png)  |   ![begin](media/begin.png)   |
|       ![P](media/P.png)       | ![setmode](media/setmode.png) |
|       ![P](media/P.png)       |  ![setout](media/setout.png)  |
| ![Control](media/Control.png) | ![forever](media/forever.png) |
| ![Control](media/Control.png) |    ![wait](media/wait.png)    |

![line5](media/line5.png)

**Conceive:**

1. **Initialization**

   Set pins and modes.

   ![3103](media/3103.png)

   <br>

   **Build blocks:**

   ① Add ![begin](media/begin.png) and ![setmode](media/setmode.png) .

   ② Set pin to 5.

   ![3105](media/3105.png)

   ③ set mode to output.

   pin mode can be one of the followings:

   - input
   - output
   - input-pullup

   ![6top](media/6top.png)
   
   Q ：Why "output"?

   A ：<span style="color: rgb(10, 10, 200);">The code is written for the mainboard.</span> For the board, pin D5 is outputting power levels (high or low) to the connected module.

   ![6bottom](media/6bottom.png)

![line3](media/line3.png)

2. **Main Code**

   Loop: LED turns on for 1s and off for 1s.

   ![3104](media/3104.png)

   <br>

   **Build blocks:**

   ① Add ![forever](media/forever.png) . Code blocks in it will run in a loop.

   ② Put ![setout](media/setout.png) into "forever". 

   This block set output power level:

   - high
   - low
   
   Set pin to 5, and set to output high.

   ③ Add a delay ![wait](media/wait.png).

   ![6top](media/6top.png)

   Q ：Why delay?

   A ：If you output a high level to LED, it will be always on. Yet, we add a delay of 1s, so it lights up for only 1s. Delay time is the ON/OFF time of LED.

   ![6bottom](media/6bottom.png)

   Set pin D5 to output high for 1s:

   ![3106](media/3106.png)

   ④ Duplicate the blocks.

   ![3107](media/3107.png)

   As follows:

   ![3108](media/3108.png)

   Modify to low. Pin D5 outputs low for 1s:

   ![3109](media/3109.png)

   The LED will circularly be on for 1s and off for 1s.

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

After uploading code, the LED module will flash with an interval of 1s (on for 1s and off for 1s).

![3102](media/3102.gif)

![4bottom](media/4bottom.png)

---

### 3.2 Hall Magnetic Sensor

![1top](media/1top.png)

![KD2101](media/KD2101.png)

This Hall sensor module is mainly composed of A3144 linear Hall components. 

Based on Hall Effect, its magnetic sensitive circuit adopts semiconductor integration technology, which is a magnetic sensing circuit composed of a voltage regulator, a Hall voltage generator, a differential amplifier, a Schmidt trigger temperature compensation circuit and an open-collector output stage. 

Its input is the magnetic induction intensity and its output is a digital voltage signal.

![1bottom](media/1bottom.png)

#### Parameters

![2top](media/2top.png)

Voltage: DC 3.3 ~ 5V 

Current: 10 mA

Maximum power: 0.05 W

Operating temperature: -10°C ~ +50°C

Dimensions: 32 x 24 x 18 mm (without housing)

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![2bottom](media/2bottom.png)

#### Principle

![3top](media/3top.png)

This Hall sensor is able to distinguish magnetic field north and south. The front of the magnetic induction element (with numbers) senses the South Pole, while its back detects the North Pole.

![3219](media/3219.png)

Modules with blue housing are digital ones, so we should connect to digital io pins of the mainboard (ports with blue).

![uno-blue](media/uno-blue.png)

In this experiment, we connect the Hall sensor module to port 2. According to the board ports view, the digital io pin at port 2 is D6.

When a magnetic field is detected, Hall sensor outputs low; When no magnetic field is detected, the sensor outputs high.

![3bottom](media/3bottom.png)

#### Wiring Diagram

![3201](media/3201.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **3.2Hall sensor.sb3** file.

![3202](media/3202.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Code Blocks**

|              Blocks               |              Code block               |
| :-------------------------------: | :-----------------------------------: |
|    ![Events](media/Events.png)    |       ![begin](media/begin.png)       |
|         ![P](media/P.png)         |     ![setmode](media/setmode.png)     |
|         ![P](media/P.png)         | ![readdigital](media/readdigital.png) |
|    ![Serial](media/Serial.png)    | ![serialbegin](media/serialbegin.png) |
|    ![Serial](media/Serial.png)    | ![serialprint](media/serialprint.png) |
| ![Operators](media/Operators.png) |           ![=](media/=.png)           |
|   ![Control](media/Control.png)   |     ![forever](media/forever.png)     |
|   ![Control](media/Control.png)   |      ![ifelse](media/ifelse.png)      |
|   ![Control](media/Control.png)   |        ![wait](media/wait.png)        |

![line5](media/line5.png)

**Conceive:**

1. **Initialization**

   Set pins and modes, initialize serial port.

   ![3203](media/3203.png)

   <br>

   **Build blocks:**

      ① Drag blocks and build as follows:

   ![3204](media/3204.png)

   ![9top](media/9top.png)

      ![serialbegin](media/serialbegin.png) : initialize serial port. Set baud rate (9600 by default). This block is indeed if you need to display messages on serial monitor. Otherwise, it fails to output.

   ![9bottom](media/9bottom.png)

   Connect Hall sensor to pin D6 on the board, and set it to input.

   ![6top](media/6top.png)

   Q ：Why "input"?

   A ：<span style="color: rgb(10, 10, 200);">The code is written for the mainboard.</span> For the Hall sensor, it is outputting power levels to the pin D6 on the board, so the board is receiving(inputting) levels.

   ![6bottom](media/6bottom.png)

![line3](media/line3.png)

2. **Main Code**

   Loop: If a magnetic field is detected, serial monitor prints *A magnetic field*. If not, it displays *There is no magnetic field*.

   ![3205](media/3205.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![3206](media/3206.png)

   ![9top](media/9top.png)

   ![readdigital](media/readdigital.png) reads digital power levels and outputs 1(high) or 0(low).

   ![serialprint](media/serialprint.png) will prints the messages in it on the serial monitor. Or you can put some variables in the printing box to display their values. Three modes are available: wrap, no wrap, HEX.

   ![9bottom](media/9bottom.png)

   Set pin to D6 and print the value without wrapping.

   ![3207](media/3207.png)

   ![6top](media/6top.png)

      Q ：Why no-wrap?

      If we set to wrap, the message will have a line break after the power level value being output.

      Wrap: 

      ![3208](media/3208.png)

      No-wrap:

      ![3209](media/3209.png)

      A ：No-wrap is more convenient for us to check the results.

   ![6bottom](media/6bottom.png)

   ② Drag blocks and build as follows:

   ![3210](media/3210.png)

   ![9top](media/9top.png)

   ![=](media/=.png): check whether the two values equal each other. If yes, outputs true.

   ![ifelse](media/ifelse.png): if else. It determines the condition is true or false. 

   True: execute codes in "if":

   ![3211](media/3211.png)

   False: execute codes in "else":

   ![3212](media/3212.png)

   ![9bottom](media/9bottom.png)

   ![3213](media/3213.png) determines whether the value read by pin D6 equals 0. Put it in "if else" block to set it to the condition.

   value of pin D6 = 0: the condition is true, execute codes in "if", and print two Space + *A magnetic field* on the serial monitor.

   value of pin D6 ≠ 0: the condition is false, execute codes in "else", and print two Space + *There is no magnetic field* .

   ![6top](media/6top.png)

      Q ：Why Space?

   The value will be too close to the contents, which is not convenient for us to check the outputs.

   Without space:

      ![3214](media/3214.png)

     With space:

      ![3215](media/3215.png)

      A ：We add a space to separate the value and contents.

   ![6bottom](media/6bottom.png)

   ③ Add a delay ![wait](media/wait.png) and set the time to 0.1s.

   ![6top](media/6top.png)

   Q ：Why delay?

   If we do not add a delay, the printing command will always run, so then the serial monitor refreshes the results very fast. A delay of 0.1s will limit the printing speed. Serial monitor refreshes outputs every 0.1s.

   A ：Limit the printing speed.

   ![6bottom](media/6bottom.png)


![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![Baud1](media/Baud1.png) and set Buadrate to 9600.

![Baud2](media/Baud2.png)

After uploading the code, when the **South Pole** of the magnet approaches to the front of the magnetic induction element, the red LED lights up and Shell prints *0  A magnetic field*; 

![3216](media/3216.png)

When the **South Pole** of the magnet approaches to its back or is away from the sensor, the red LED goes off, and Shell prints *1  There is no magnetic field* .

![3217](media/3217.png)

Put the **North Pole** of the magnet to the back of the element, the red LED lights up and Shell prints *0  A magnetic field*; 

![3220](media/3220.png)

When the **North Pole** of the magnet approaches to the front of the sensor or is away from it, the red LED goes off, and Shell prints *1  There is no magnetic field*.

![3221](media/3221.png)

![3218](media/3218.gif)

![4bottom](media/4bottom.png)

---

### 3.3 Passive Buzzer

![1top](media/1top.png)

![KD2121](media/KD2121.png)

Buzzer is an integrated structure of electronic sound device, which is powered by DC voltage. In application, it is widely used in computers, printers, copiers, alarms, electronic toys, automotive electronic equipment, telephones and timers. 

Buzzers can be divided into active ones(built-in drive circuits) and passive ones(external drive) according to that whether they includes an excitation source.

Active buzzers contain oscillation source inside, which can sound at a fixed frequency once be triggered. They are convenient in program control and features high sound pressure.

Passive ones, however, do not include oscillating sources. If we directly power a passive buzzer via DC voltage, it will emit no sound. According to needs, we generally drive through square waves, whose frequency determines the sound tones.

**To sum up, The active buzzer contains a vibration source, and its sound frequency is fixed. Yet there is no vibration source inside the passive one, so it must be driven by square waves whose frequency can be changed to control sounds.**

![1bottom](media/1bottom.png)

#### Parameters

![2top](media/2top.png)

Operating voltage: DC 3.3 ~ 5V 

Operating temperature: -10°C ~ +50°C

Control signal: Digital signal

Dimensions: 48 x 24 x 18 mm (without housing)

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![2bottom](media/2bottom.png)

#### Principle

![3top](media/3top.png)

Music is an invisible art. It is a language that narrates emotions and thoughts. 

The foundation of music, as we all know, is note. We can compose a variety of melodies and rhythms with different notes. Of all the notes, the most basic are seven:

![3301](media/3301.png)

We can compose a variety of melodies and rhythms with these notes.

Passive buzzer module must be drive by square waves to emit sound. We can change the duty cycle of PWM to control square waves.

- The greater the duty cycle is, the lauder the sound will be.

And the tones vary from different frequency of PWM.

- The higher the frequency is, the higher the tone will be.

![peg](media/peg.png)

![line3](media/line3.png)

**What is PWM?**

PWM (Pulse width modulation) simulates the change of analog signal through digital signal.

Pulse width is the high level in a complete square wave cycle. So, pulse width modulation is to adjust the high level(of course, in other words, low level is also adjusted).

![3302](media/3302.png)

- **PWM frequency**: the number of times the signal going from high level to low level and back to high level in 1 second (one cycle), that is, how many cycles there are in a second.

  **Unit**: Hz

  **Expression**: 50Hz 100Hz

- **PWM cycle**

	$ T= \frac {1}{f}$      $ Cycle= \frac {1}{frequency}$

	If the frequency is 50Hz, the cycle will be 20ms, i.e., there are 50 PWM cycles in one second.

- **PWM duty cycle**: the ratio of high level time to the whole cycle time.

	- Unit: %(1% ~ 100%)
	- Cycle: The time of a pulse signal. The number of cycles in 1s equals the frequency.
	- Pulse width time: high level time.
	
	![3303](media/3303.gif)
	
	<center>The relationship between duty cycle and LED brightness<center>

The longer the high level time is, the greater the duty cycle will be, and the brighter the LED will be.

**The PWM frequency corresponding to notes**:

![3304](media/3304.png)

![line3](media/line3.png)

Modules with blue housing are digital ones, so we should connect to digital io pins of the mainboard (ports with blue).

![uno-blue](media/uno-blue.png)

In this experiment, we connect the passive buzzer to port 3. According to the board ports view, the digital io pin at port 3 is D3.

![3bottom](media/3bottom.png)

#### Wiring Diagram

![3305](media/3305.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **3.3Passive buzzer.sb3** file.

![3306](media/3306.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Code Blocks**

|            Blocks             |              Code block               |
| :---------------------------: | :-----------------------------------: |
|  ![Events](media/Events.png)  |       ![begin](media/begin.png)       |
|  ![Buzzer](media/Buzzer.png)  | ![Buzzer_freq](media/Buzzer_freq.png) |
| ![Control](media/Control.png) |     ![forever](media/forever.png)     |
| ![Control](media/Control.png) |        ![wait](media/wait.png)        |

![line5](media/line5.png)

**Conceive:**

Add library first. Click ![add](media/add.png) and find **Passive buzzer** to add in extension.

![3313](media/3313.png)

Click  **Back**.

![3314](media/3314.png)

Successfully load.

![3315](media/3315.png)

**Main Code**

Loop: play tones of C, D, E, F, G, A, B, each tone plays 200ms.

![3307](media/3307.png)

<br>

**Build blocks:**

① Build blocks as follows:

![3308](media/3308.png)

Set pin to 3 and frequency to NOTE_C5, add a delay of 0.2s.

![3309](media/3309.png)

② Duplicate this block.

![3310](media/3310.png)

As follows:

![3311](media/3311.png)

Duplicate six times, as follows:

![3312](media/3312.png)

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

After uploading the code, the buzzer will circularly play tones(C, D ,E, F, G, A, B).

![4bottom](media/4bottom.png)

#### Extension

![7top](media/7top.png)

Congratulations! You have played these basic notes successfully! Now let's try to compose a beautiful music and play with this passive buzzer!

Open **3.3Music.sb3** file.

![3316](media/3316.png)

Choose a music you like.

![3317](media/3317.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

Upload! And you will hear the music!

![3318](media/3318.gif)

![7bottom](media/7bottom.png)


---

### 3.4 XHT11 Temperature and Humidity Sensor

![1top](media/1top.png)

![KD2095 ](media/KD2095.png)

XHT11 sensor is a low-cost and entry-level temperature and humidity sensor, which consists of a resistive humidity sensor and an NTC temperature sensor. It is designed 4-pin single-row pin and adopts single-wire serial interface, so we just add the appropriate pull-up resistance to read values. Moreover, its signal transmission distance can reach more than 20 meters.

![1bottom](media/1bottom.png)

#### Parameters

![2top](media/2top.png)

Operating voltage ：DC 3.3 ~ 5V 

Operating current: 2.1 mA

Maximum power: 0.015 W

Humidity detection range: 5 ~ 95%RH (accuracy of ±5%RH under 25°C)

Temperature detection range: -25°C ~ +60°C

Operating temperature: -10°C ~ +50°C

Input signal: Digital signal

Dimensions: 48 x 24 x 18 mm (without housing)

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![2bottom](media/2bottom.png)

#### Principle

![3top](media/3top.png)

Modules with blue housing are digital ones, so we should connect to digital io pins of the mainboard (ports with blue).

![uno-blue](media/uno-blue.png)

In this experiment, we connect the passive buzzer to port 4. According to the board ports view, the digital io pin at port 4 is D2.

![3bottom](media/3bottom.png)

#### Wiring Diagram

![3401](media/3401.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **3.4Humiture.sb3** file.

![3402](media/3402.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Code Blocks**

|            Blocks             |              Code block               |
| :---------------------------: | :-----------------------------------: |
|  ![Events](media/Events.png)  |       ![begin](media/begin.png)       |
|  ![Serial](media/Serial.png)  | ![serialbegin](media/serialbegin.png) |
|  ![Serial](media/Serial.png)  | ![serialprint](media/serialprint.png) |
|     ![DHT](media/DHT.png)     |     ![dht-pin](media/dht-pin.png)     |
|     ![DHT](media/DHT.png)     |       ![dht-t](media/dht-t.png)       |
|     ![DHT](media/DHT.png)     |       ![dht-h](media/dht-h.png)       |
| ![Control](media/Control.png) |     ![forever](media/forever.png)     |
| ![Control](media/Control.png) |        ![wait](media/wait.png)        |

![line5](media/line5.png)

**Conceive:**

Add library first. Click ![add](media/add.png) to load **DHT sensor** .

![3403](media/3403.png)


1. **Initialization**

   Initialize serial port to prepare for the display of temperature and humidity value.

   ![3404](media/3404.png)

![line3](media/line3.png)

2. **Main Code**

   Loop: read and print the temperature and humidity value every 0.5s.

   ![3405](media/3405.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![3406](media/3406.png)

   ![9top](media/9top.png)

   ![dht-pin](media/dht-pin.png) set the sensor pin.

   ![9bottom](media/9bottom.png)

   ② Drag blocks and build as follows:

   ![3407](media/3407.png)

   ![9top](media/9top.png)

   ![dht-t](media/dht-t.png) read the temperature value in the unit of °C or °F.

   ![9bottom](media/9bottom.png)
   
   Herein, print "temperature:" + measured actual temperature value + " °C" without wrapping. There is a space before °C, which is convenience for us to check results.
   
   ③ Drag blocks and build as follows:
   
   ![3408](media/3408.png)
   
   ![9top](media/9top.png)
   
   ![dht-t](media/dht-h.png) reads the humidity value.
   
   ![9bottom](media/9bottom.png)
   
   This code prints the actual humidity value in the unit of " %" without wrapping. There is also a space before %. What follows " %" is a line break to print next group of values.
   
   ④ Add a delay ![wait](media/wait.png) and set it to 0.5, so the results will be refreshed every 0.5s.

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![Baud1](media/Baud1.png) and set Buadrate to 9600.

![Baud2](media/Baud2.png)

After uploading the code, the serial monitor prints the actual temperature and humidity value every 0.5s.

![3409](media/3409.png)

Blow to the XHT11 sensor and you will see both temperature and humidity values rise.

![3410](media/3410.png)

![3411](media/3411.png)



![4bottom](media/4bottom.png)

---

### 3.5 Steam Sensor

![1top](media/1top.png)

![KD2084](media/KD2084.png)

Unlike the previous modules, the steam sensor is an analog module rather than a digital one.

What is the difference? For digital modules, they only output high(5V) or low(0V); while analog ones are able to output or input intermediate voltage values through ADC analog ports on the board.

![1bottom](media/1bottom.png)

#### Parameters

![2top](media/2top.png)

Operating voltage: DC 3.3 ~ 5V 

Operating current: 1.5 mA

Maximum power: 0.075 W

Operating temperature: -10°C ~ +50°C

Dimensions: 48 x 24 x 18 mm (without housing)

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![2bottom](media/2bottom.png)

#### Principle

![3top](media/3top.png)

The steam sensor measures the amount of water through its exposed lines. The water will connect these lines. The more amount of water is, the wider the conductive area will be connected, and the higher the output voltage will be.

With the change of amount of water, the voltage (0 ~ 5V) detected by the analog port will change accordingly. This change is continuous, which means it can be any value within 0 ~ 5V.

<span style="color: rgb(10, 10, 200);">The board can only process digital signals, so we need to convert analog signals in to digital ones. Thus, an ADC(Analog to Digital Converter) acquisition is required.</span>

![peg](media/peg.png)

![line3](media/line3.png)

**What is ADC?**

ADC(Analog to Digital Converter) converts analog values to digital ones. The ADC acquisition is integrated in our board, so you can call it directly. 

**KidsIOT ADC Parameters**

1. Reference voltage: 5V

2. Resolution: 10bit

	A n-bit ADC means this ADC contains 2ⁿ scales.

	10-bit ADC contains $2^{10}=1024$ scales, and it outputs totally 1024 digital values (including from 0～ 1024), each scale is $\frac{5}{1023}≈0.00489(V)$ .

3. General ADC input voltage calculation: 

	<font face="courier New" color="black" size=6>$ Vin= \frac {AVDD_{ADC}}{2^{Resolution Bit}-1}*ReadData$</font> 

4. $AVDD_{ADC}$：Reference voltage

![line3](media/line3.png)

Modules with red housing are analog ones, so we should connect to analog io pins of the mainboard (ports with red).

![uno-red](media/uno-red.png)

In this experiment, we connect the module to port 4. According to the board ports view, the analog io pin at port 4 is A2.

![3bottom](media/3bottom.png)

#### Wiring Diagram

![3501](media/3501.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **3.5Steam sensor.sb3** file.

![3502](media/3502.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Code Blocks**

|              Blocks               |               Code block                |
| :-------------------------------: | :-------------------------------------: |
|    ![Events](media/Events.png)    |        ![begin](media/begin.png)        |
|         ![P](media/P.png)         |      ![setmode](media/setmode.png)      |
|         ![P](media/P.png)         |   ![readanalog](media/readanalog.png)   |
|    ![Serial](media/Serial.png)    |  ![serialbegin](media/serialbegin.png)  |
|    ![Serial](media/Serial.png)    |  ![serialprint](media/serialprint.png)  |
|      ![Vari](media/Vari.png)      | ![variablename](media/variablename.png) |
|      ![Vari](media/Vari.png)      |  ![setvariable](media/setvariable.png)  |
|      ![Vari](media/Vari.png)      |     ![variable](media/variable.png)     |
| ![Operators](media/Operators.png) |       ![divide](media/divide.png)       |
| ![Operators](media/Operators.png) |     ![multiply](media/multiply.png)     |
|   ![Control](media/Control.png)   |      ![forever](media/forever.png)      |
|   ![Control](media/Control.png)   |         ![wait](media/wait.png)         |

![line5](media/line5.png)

**Conceive:**

1. **Initialization**

   Set pins and modes, initialize the serial port. Create a variable to store the analog value of steam sensor.

   ![3503](media/3503.png)
   
   ![9top](media/9top.png)
   
   ![variablename](media/variablename.png) defines parameters of a variable.
   
   - ![3610](media/3610.png)
   
     Define a global or local variable.
   
   - ![3611](media/3611.png)
   
     Define the variable type.
   
   - ![3612](media/3612.png)
   
     Name the variable.
   
   - ![3613](media/3613.png)
   
     Assign an initial value to the variable.
   
   ![9bottom](media/9bottom.png)
   
   ![3508](media/3508.png)
   
   Create a float variable named *Water_value* to store the analog value read by the steam sensor, and assign an initial value of 0 to it.

![line3](media/line3.png)

2. **Main Code**

   Loop: print the analog value read by the sensor and the voltage converted from the analog value. The results will be refreshed every 0.1s.

   ![3504](media/3504.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![3505](media/3505.png)
   
   ![9top](media/9top.png)
   
   ![setvariable](media/setvariable.png) sets variable and assigns value to it.
   
   ![readanalog](media/readanalog.png) reads analog values.
   
   ![9bottom](media/9bottom.png)
   
   Connect steam sensor to pin A2; Read the value of pin A2 and assign it to *Water_value*.
   
   ② Drag blocks and build as follows:
   
   ![3506](media/3506.png)
   
   ![9top](media/9top.png)
   
   ![variable](media/variable.png) represents the variable. 
   
   ![multiply](media/multiply.png) : the two value will be multiplied. It outputs the result.
   
   ![divide](media/divide.png) : the left value will divide by the right value. It outputs the result.
   
   ![9bottom](media/9bottom.png)
   
   The calculation of actual voltage value:
   
   ![3507](media/3507.png)
   
   The output value will be a input voltage value in the unit of V.
   
   ③ Add a delay ![wait](media/wait.png) and set it to 0.1s. The results will be refreshed every 0.1s.

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![Baud1](media/Baud1.png) and set Buadrate to 9600.

![Baud2](media/Baud2.png)

After uploading the code, the monitor outputs the detected analog values of water/vapor and the converted voltage values.

![3509](media/3509.png)

The more the amount of water is / the wetter the air is, the greater the analog and voltage value will be.

![3510](media/3510.png)

Breath on the detection area, or touch it with a wet tissue, and you will see the analog value ans voltage will both increase.

<span style="color: rgb(2550, 10, 50);">**ATTENTION: Be careful when using water, please do not to drip to any other place outside the detection area to aviod a short circuit.**</span>

![3511](media/3511.png)

![4bottom](media/4bottom.png)

---

###  3.6 Flame Sensor

![1top](media/1top.png)

![KD2097](media/KD2097.png)

Since a far-infrared flame probe is reserved, the flame sensor is particularly sensitive to the flame spectrum, so this sensor is an essential part of the fire-fighting robot to find the fire source.

![1bottom](media/1bottom.png)

#### Parameters

![2top](media/2top.png)

Operating voltage: DC 3.3 ~ 5V 

Current: 1.2 mA

Maximum power: 0.006 W

Detection flame wavelength: 760 nm ~ 1100 nm

Detection range: 0 ~ 60 mm

Detection Angle: about 60°

Operating temperature: -10°C ~ +50°C

Dimensions: 48 x 24 x 18 mm

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![2bottom](media/2bottom.png)

#### Principle

![3top](media/3top.png)

The sensitive element of the sensor is a special infrared receiving diode, which is very sensitive to the infrared generated by the flame. It detects flame by converting the brightness of the flame into power level signals.

Modules with red housing are analog ones, so we should connect to analog io pins of the mainboard (ports with red).

![uno-red](media/uno-red.png)

In this experiment, we connect the module to port 6. According to the board ports view, the analog io pin at port 6 is A1.

![3bottom](media/3bottom.png)

#### Wiring Diagram

![3601](media/3601.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **3.6Flame sensor.sb3** file.

![3602](media/3602.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Code Blocks**

|              Blocks               |               Code block                |
| :-------------------------------: | :-------------------------------------: |
|    ![Events](media/Events.png)    |        ![begin](media/begin.png)        |
|         ![P](media/P.png)         |      ![setmode](media/setmode.png)      |
|         ![P](media/P.png)         |   ![readanalog](media/readanalog.png)   |
|      ![Vari](media/Vari.png)      | ![variablename](media/variablename.png) |
|      ![Vari](media/Vari.png)      |  ![setvariable](media/setvariable.png)  |
|      ![Vari](media/Vari.png)      |     ![variable](media/variable.png)     |
|    ![Serial](media/Serial.png)    |  ![serialbegin](media/serialbegin.png)  |
|    ![Serial](media/Serial.png)    |  ![serialprint](media/serialprint.png)  |
| ![Operators](media/Operators.png) |       ![divide](media/divide.png)       |
| ![Operators](media/Operators.png) |     ![multiply](media/multiply.png)     |
| ![Operators](media/Operators.png) |         ![less](media/less.png)         |
|   ![Control](media/Control.png)   |      ![forever](media/forever.png)      |
|   ![Control](media/Control.png)   |       ![ifelse](media/ifelse.png)       |
|   ![Control](media/Control.png)   |         ![wait](media/wait.png)         |

![line5](media/line5.png)

**Conceive:**

1. **Initialization**

   Set pins and modes, initialize the serial port and create variables.

   ![3603](media/3603.png)

   ![3614](media/3614.png)

   Create a float variable named *Flame_value* to store the analog value of the flame sensor, assign an initial value of 0.

   ![3615](media/3615.png)

   Create a float variable named *Voltage* to store the actual voltage value, assign an initial value of 0.


![line3](media/line3.png)

2. **Main Code**

   Loop: print the analog value read by the sensor and the voltage converted from the analog value. The results will be refreshed every 0.1s.

   ![3604](media/3604.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![3605](media/3605.png)

   ![9top](media/9top.png)

   ![setvariable](media/setvariable.png) set variable and assign to it.

   ![variable](media/variable.png) is a variable block.

   ![9bottom](media/9bottom.png)

   Connect the flame sensor to pin A1, read the analog value of pin A1 and assign it to the variable *Flame_value*. 

   Calculate the actual voltage value and assign it to *Voltage*.

   ② Drag blocks and build as follows:

   ![3607](media/3607.png)

   Output the analog value and voltage value of the flame sensor.

   ③ Drag blocks and build as follows:

   ![3608](media/3608.png)

   ![9top](media/9top.png)
   
   ![less](media/less.png) determines whether left value of less than the right one. If yes, the condition will be output true.
   
   ![9bottom](media/9bottom.png)
   
   When flame is detected, the voltage decrease. The brighter the flame is, the lower the voltage will be output. 
   
   In this experiment, we set the threshold voltage value to 4 (you can modify this value according to needs), so when the voltage is lower than 4, the flame is detected.
   
   We add an **if else** block to determine whether the voltage output is lower than 4. The voltage is a float value so it is more accurate.
   
   If voltage < 4, the serial monitor will display *Flame detected!* ; When voltage ≥ 4, it will prints *Nothing* .
   
   ④ Add a delay ![wait](media/wait.png) and set it to 0.1. The results will be refreshed every 0.1s.

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![Baud1](media/Baud1.png) and set Buadrate to 9600.

![Baud2](media/Baud2.png)

After uploading the code, *Flame detected!* will be displayed on the serial monitor when the flame sensor detects flame.

If no flame is detected, the serial monitor shows *Nothing*.

![3609](media/3609.png)

![4bottom](media/4bottom.png)

---

### 3.7 Sound Sensor

![1top](media/1top.png)

Old:

![KD2098](media/KD2098.png)

New:

![KD2098BG](media/KD2098BG.png)

The sound sensor acts as a microphone that can capture sound information in the environment.

It is consists of a sensitive capacitor microphone for detecting sound and an amplification circuit. It works based on the propagation and vibration of sound. When sound travels near the sensor, the sound wave causes the sensor to vibrate. Then, the sensor converts sound vibrations into electrical signals and sends them for further processing or analysis.

![1bottom](media/1bottom.png)

#### Parameters

![2top](media/2top.png)

Operating voltage: DC 3.3 ~ 5V 

Current: 15 mA

Maximum power: 0.075 W

Operating temperature: -10°C ~ +50°C

Dimensions: 48 x 24 x 18 mm

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![2bottom](media/2bottom.png)

#### Principle

![3top](media/3top.png)

When you speak loudly or play music to the MIC, these sound signals are converted into electrical ones, which are output at analog ports.

The amplifier circuit on the module amplifies the sound detected by the MIC. We can adjust the amplification by rotating the potentiometer. It is the maximum when we adjust the potentiometer clockwise to the end.

![3703](media/3703.png)

Modules with red housing are analog ones, so we should connect to analog io pins of the mainboard (ports with red).

![uno-red](media/uno-red.png)

In this experiment, we connect the module to port 7. According to the board ports view, the analog io pin at port 7 is A0.

![3bottom](media/3bottom.png)

#### Wiring Diagram

![3708](media/3708.png)

![3701](media/3701.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **3.7Sound sensor.sb3** file.

![3702](media/3702.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Code Blocks**

|            Blocks             |              Code block               |
| :---------------------------: | :-----------------------------------: |
|  ![Events](media/Events.png)  |       ![begin](media/begin.png)       |
|       ![P](media/P.png)       |     ![setmode](media/setmode.png)     |
|       ![P](media/P.png)       |  ![readanalog](media/readanalog.png)  |
|  ![Serial](media/Serial.png)  | ![serialbegin](media/serialbegin.png) |
|  ![Serial](media/Serial.png)  | ![serialprint](media/serialprint.png) |
| ![Control](media/Control.png) |     ![forever](media/forever.png)     |
| ![Control](media/Control.png) |        ![wait](media/wait.png)        |

![line5](media/line5.png)

**Conceive:**

1. **Initialization**

   Set pins and modes, initialize the serial port.

   ![3704](media/3704.png)

![line3](media/line3.png)

2. **Main Code**

   Loop: print the analog value read by the sound sensor every 0.1s.

   ![3705](media/3705.png)

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![Baud1](media/Baud1.png) and set Buadrate to 9600.

![Baud2](media/Baud2.png)

After uploading the code, speak to the MIC, and monitor will display the analog value of sound volume that is detected by the sound sensor.

![3706](media/3706.png)

![4bottom](media/4bottom.png)

---

### 3.8 Ultraviolet Sensor

![1top](media/1top.png)

![KD2102](media/KD2102.png)

In the solar spectrum, the frequency of ultraviolet is higher than that of visible light, so it is invisible. 

Ultraviolet light can be divided into UVA, UVB, UVC, EUV. Among them, UVA causes tanning; UVB may burn skin due to its shorter wavelength; UVC is normally blocked by the ozone layer. 

Through ultraviolet radiation, the skin will produce more melanin, which is distributed upward into the cuticle of the epidermis to form brown spots. So it is the biggest culprit of skin wrinkles, aging or sagging.

But it's not all bad. When ultraviolet light hits the body, it can promote the synthesis of vitamin D to prevent rickets. Besides, it harbors bactericidal efficacy, so some hospitals disinfect by ultraviolet light. In spite of its benefits, too strong ultraviolet will harm the human body, leading to a skin cancer.

![1bottom](media/1bottom.png)

#### Parameters

![2top](media/2top.png)

Operating voltage: DC 3.3 ~ 5V 

Operating current: 1 mA

Operating power: 0.005 W

Peak wavelength: 355 nm

Peak response rate: 0.18A/W (at 355 nm)

Spectral response range: 280 ~ 370 nm

Active region: 0.076 mm²

Responsivity: 0.14 A/W (test under λ = 300 nm, U~R~ = 0 V)

Dark current: 1nA (test under U~R~ = 0.1 V )

Light current: 113 nA (test under UVA light, 1 mW/cm); 26 nA (test under 1 UVI)

Temperature coefficient: 0.08 %/°C 

Operating temperature: -10°C ~ +50°C

Output signal: Analog signal

Dimensions: 48 x 24 x 18 mm (without housing）

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![2bottom](media/2bottom.png)

#### Principle

![3top](media/3top.png)

This ultraviolet sensor measures the intensity of ultraviolet light and converts it into electrical outputs.

The relationship between the output voltage of the UV sensor and the UV index:

![3806](media/3806.png)

<center>Comparison Table of Voltage and UV Index</center>

We can have a clearly look of the UV index corresponding to the output voltage. <span style="color: rgb(10, 10, 200);">The voltage is in the unit of mV.</span>

Modules with red housing are analog ones, so we should connect to analog io pins of the mainboard (ports with red).

![uno-red](media/uno-red.png)

In this experiment, we connect the module to port 8. According to the board ports view, the analog io pin at port 8 is A7.

![3bottom](media/3bottom.png)

#### Wiring Diagram

![3801](media/3801.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **3.8Solar ultraviolet sensor.sb3** file.

![3802](media/3802.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Code Blocks**

|              Blocks               |               Code block                |
| :-------------------------------: | :-------------------------------------: |
|    ![Events](media/Events.png)    |        ![begin](media/begin.png)        |
|         ![P](media/P.png)         |      ![setmode](media/setmode.png)      |
|         ![P](media/P.png)         |   ![readanalog](media/readanalog.png)   |
|      ![Vari](media/Vari.png)      | ![variablename](media/variablename.png) |
|      ![Vari](media/Vari.png)      |  ![setvariable](media/setvariable.png)  |
|      ![Vari](media/Vari.png)      |     ![variable](media/variable.png)     |
|    ![Serial](media/Serial.png)    |  ![serialbegin](media/serialbegin.png)  |
|    ![Serial](media/Serial.png)    |  ![serialprint](media/serialprint.png)  |
| ![Operators](media/Operators.png) |       ![divide](media/divide.png)       |
| ![Operators](media/Operators.png) |     ![multiply](media/multiply.png)     |
| ![Operators](media/Operators.png) |         ![less](media/less.png)         |
| ![Operators](media/Operators.png) |      ![greater](media/greater.png)      |
| ![Operators](media/Operators.png) |          ![and](media/and.png)          |
|   ![Control](media/Control.png)   |      ![forever](media/forever.png)      |
|   ![Control](media/Control.png)   |           ![if](media/if.png)           |
|   ![Control](media/Control.png)   |         ![wait](media/wait.png)         |

![line5](media/line5.png)

**Conceive:**

1. **Initialization**

   Initialize serial port.

   Create a float variable *voltage* to store the input voltage of the ultraviolet sensor. Assign an initial value of 0 to it.

   Create an integer variable *uv* to store the detected UV index. Assign an initial value of 0 to it.

   ![3803](media/3803.png)

   ![line3](media/line3.png)

2. **Main Code**

   Loop: print the analog value read by the sensor and the voltage converted from the analog value. The results will be refreshed every 0.1s.

   ![3804](media/3804.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![3805](media/3805.png)

   Connect the UV sensor to pin A7, read the analog value of pin A7 and convert it into voltage(V).

   ![3807](media/3807.png)

   The voltage unit in the Comparison Table is millivolt(mV), so we convert the analog value read by the sensor into voltage in mV. We only need to multiply the value by 1000.

   ![3808](media/3808.png)

   Assign the converted value to variable *voltage*.

   ② Drag blocks and build as follows:

   ![3809](media/3809.png)

   ![9top](media/9top.png)

   ![if](media/if.png)

   If the condition is True, execute the blocks in "if".

   If the condition is False, skip this block.

   ![9bottom](media/9bottom.png)

   If the voltage is lower than 50mV, variable uv = 0.

   ③ Drag blocks and build as follows:

   ![3810](media/3810.png)

   ![9top](media/9top.png)

   ![greater](media/greater.png) determines whether the left value is greater than the right value. If yes, the condition will be output true.

   ![and](media/and.png): Only when the two conditions are both satisfied, it outputs True.

   ![9bottom](media/9bottom.png)

   When the voltage is greater than 50 but lower than 227, variable uv = 1.

   ④ Duplicate the block.
   
   ![3811](media/3811.png)
   
   As follows:
   
   ![3812](media/3812.png)
   
   Duplicate for 10 times and set the condition according to the Comparison Table:
   
   If voltage < 50 is True, uv = 0.
   
   If voltage > 50 and voltage < 227, uv = 1.
   
   If voltage > 227 and voltage < 318, uv = 2.
   
   ... ...
   
   If voltage > 976 and voltage < 1079, uv = 10.
   
   If voltage > 1079, uv = 11.
   
   ![3813](media/3813.png)
   
   We adopt **if** block to determine the range of the UV index.
   
   ⑤ Put into **forever**, as follows:
   
   ![3814](media/3814.png)
   
   Serial monitor prints the voltage value and UV index and refreshes the results every 0.1s.

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![Baud1](media/Baud1.png) and set Buadrate to 9600.

![Baud2](media/Baud2.png)

After uploading the code, the monitor prints the UV index and the voltage value (mV) converted from analog values of the sensor.

![3815](media/3815.png)

![4bottom](media/4bottom.png)

---

### 3.9 Traffic Light Module

![1top](media/1top.png)

![KD2080](media/KD2080.png)

A traffic light acts as a signal that commands the traffic operation, which is generally composed of red, green and yellow light. Red indicates traffic-prohibited, green means traffic-permitted, and yellow is a warning signal.

This traffic light module is also composed of red LED, yellow and green LED, whose working principle is consistent with that of white LED module.

![1bottom](media/1bottom.png)

#### Parameters

![2top](media/2top.png)

Operating voltage: DC 3.3 ~ 5V 

Operating current: 40 mA

Maximum power: 0.2 W

Operating temperature: -10°C ~ +50°C

Dimensions: 48 x 24 x 18 mm (without housing)

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![2bottom](media/2bottom.png)

#### Principle

![3top](media/3top.png)

The port of this module is in white, so we need to connect it to the white ports on the board.

![uno-white](media/uno-white.png)

In this experiment, we connect the module to port 9. According to the order of the pins, the red LED is connected to pin D9, yellow to pin D10, and green to D11.

When the mainboard inputs high(1) to the module, the connected LED will light up. If it is low(0), the related LED will go off.

![3bottom](media/3bottom.png)

#### Wiring Diagram

![3901](media/3901.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **3.9Traffic light module.sb3** file.

![3902](media/3902.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Code Blocks**

|            Blocks             |          Code block           |
| :---------------------------: | :---------------------------: |
|  ![Events](media/Events.png)  |   ![begin](media/begin.png)   |
|       ![P](media/P.png)       | ![setmode](media/setmode.png) |
|       ![P](media/P.png)       |  ![setout](media/setout.png)  |
| ![Control](media/Control.png) | ![forever](media/forever.png) |
| ![Control](media/Control.png) |    ![wait](media/wait.png)    |
| ![Control](media/Control.png) |  ![repeat](media/repeat.png)  |

![line5](media/line5.png)

**Conceive:**

1. **Initialization**

   Set pins and modes.

   ![3903](media/3903.png)


![line3](media/line3.png)

2. **Main Code**

   Loop: red LED lights up for 5s; yellow LED blinks for 3 times; green LED lights up for 5s.

   ![3904](media/3904.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![3905](media/3905.png)

   Set pin D9 to output high for 5s and then output low: red LED lights up for 5s and goes off.

   ② Drag blocks and build as follows:

   ![3906](media/3906.png)

   ![9top](media/9top.png)

   ![repeat](media/repeat.png) : codes in this block will run repeatedly, and the times can be set.

   ![9bottom](media/9bottom.png)

   ![3907](media/3907.png)

   The yellow LED turns on for 0.5s and off for 0.5s (blinks for 1s).

   ![3908](media/3908.png)

   Set the times to 3, so the yellow LED blinks for 3 times.

   ③ Drag blocks and build as follows:

   ![3909](media/3909.png)

   The green LED lights up for 5s and goes off.

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

After uploading the code, repeat these actions: the red LED lights up for 5s, yellow one blinks for 3 times and green LED lights up for 5s. 

![3902](media/3902.gif)

![4bottom](media/4bottom.png)

---

### 3.10 LPS331APTR Air Pressure Sensor

![1top](media/1top.png)

![KD2117](media/KD2117.png)

Air pressure effects human health physiologically and psychologically.

Low pressure, on the one hand, influences the supply of oxygen. When human body lacks of oxygen, especially the brain, symptoms such as dizziness, headache, nausea, vomiting and weakness may be developed. On the other hand, impairments may also located in the nervous system. Even lung edema and coma may occur, which is commonly known as the "mountain reaction".

High pressure is also having a deleterious effect. It may lead to tinnitus, dizziness, and even the rupture of the eardrum; Decompression sickness can occur if decompression is not done properly after working in a high pressure environment.

Beyond that, air pressure will also change people's psychological moods, causing depressed emotions.



![1bottom](media/1bottom.png)

#### Parameters

![2top](media/2top.png)

Operating voltage: DC 3.3 ~ 5V

Operating current: 30 uA

Maximum power: 0.000015 W

Working pressure range: 260 ~ 1260 mbar

Operating temperature: -10°C ~ +50°C

Dimensions: 48 x 24 x 18 mm (without housing)

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![2bottom](media/2bottom.png)

#### Principle

![3top](media/3top.png)

LPS331APTR module is with green housing, which is an I2C communication sensor, so we should connect to ports with green on the board.

In this experiment, we connect it to port 5.

![uno-green](media/uno-green.png)

Before using, we need to import LPS331AP library.

![3bottom](media/3bottom.png)

#### Wiring Diagram

![31001](media/31001.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **3.10Air pressure detection.sb3** file.

![31002](media/31002.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Code Blocks**

|             Blocks              |           Code block            |
| :-----------------------------: | :-----------------------------: |
|   ![Events](media/Events.png)   |    ![begin](media/begin.png)    |
| ![Pressure](media/Pressure.png) | ![LPS331AP](media/LPS331AP.png) |
|  ![Control](media/Control.png)  |  ![forever](media/forever.png)  |
|  ![Control](media/Control.png)  |     ![wait](media/wait.png)     |

![line5](media/line5.png)

**Conceive:**

Add library first. Click ![add](media/add.png) to load **lps331ap** .

![31003](media/31003.png)

1. **Initialization**

   Initialize the serial port.

   ![31004](media/31004.png)


![line3](media/line3.png)

2. **Main Code**

   Loop: print the air pressure value and temperature value read by the LPS331APTR sensor. The results will be refreshed every 0.1s.

   ![31005](media/31005.png)


![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![Baud1](media/Baud1.png) and set Buadrate to 9600.

![Baud2](media/Baud2.png)

After uploading the code, the monitor outputs the pressure and temperature value and refreshes them every 0.1s.

![31007](media/31007.png)

Touch the sensing area with your finger, and you will see the temperature value rises.

![31006](media/31006.png)

![31008](media/31008.png)

![4bottom](media/4bottom.png)

---

## 4. Comprehensive Experiments

### 4.1 Rain Detection

This station monitors weather conditions in real time.

In this experiment, we combine a steam sensor and a passive buzzer to achieve a rain detection function for this mini meteorological station. When the steam sensor detects rain, the buzzer alarms. 

#### Flow

![4101](media/4101.png)

#### Assembly

![line1](media/line1.png)

**Required Parts**

![41_00](media/41_00.png)

![line1](media/line1.png)

**Step 1**

![41_01](media/41_01.png)

![line1](media/line1.png)

**Step 2**

![41_02](media/41_02.png)

![line1](media/line1.png)

**Step 3**

![41_03](media/41_03.png)

![line1](media/line1.png)

**Step 4**

![41_04](media/41_04.png)

![line1](media/line1.png)

**Step 5**

![41_05](media/41_05.png)

![line1](media/line1.png)

**Step 6**

![41_06](media/41_06.png)

![line1](media/line1.png)

**Step 7**

![41_07](media/41_07.png)

![line1](media/line1.png)

**Step 8**

![41_08](media/41_08.png)

![line1](media/line1.png)

**Completed**

![41_09](media/41_09.png)

![line1](media/line1.png)

#### Wiring Diagram

![4102](media/4102.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **4.1Rain detection.sb3** file.

![4103](media/4103.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Conceive:**	

Set a threshold of voltage to determine the water volume. When there is too much water, the voltage exceeds the threshold, rain is detected, and the buzzer alarms. The buzzer will stop alarming when the voltage is lower than the threshold.

![line2](media/line2.png)

**Code structure:**

1. Initialization. Set the pins of the steam sensor and the passive buzzer, set the voltage value of a single scale, and set the frequency of the passive buzzer.

   ![4104](media/4104.png)

2. Loop:

   Print the analog value and voltage of the steam sensor.

   Determine whether the voltage exceeds 1 (<span style="color: rgb(10, 10, 200);">Herein, we set 1 as the threshold, which is adjustable according to needs</span>).

   - voltage > 1: buzzer alarms.
   - voltage ≤ 1: buzzer does not emit sounds.

   ![4105](media/4105.png)

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

After uploading the code, the steam sensor will detects the ambient water volume and converts it to a voltage output. When the voltage is greater than 1, the buzzer alarms. If not, the buzzer will not emit sounds.

<span style="color: rgb(2550, 10, 50);">**ATTENTION: Be careful when using water, please do not to drip to any other place outside the detection area to aviod a short circuit.**</span>

![4106](media/4106.gif)

![4bottom](media/4bottom.png)

---

### 4.2 Fire Alarm

The fire alarm system of the station can effectively prevent and deal with forest fires.

In this experiment, we build a fire alarm with a flame sensor and a passive buzzer. When flame is detected, the buzzer will emit sounds for alarming. 

#### Flow

![4201](media/4201.png)

#### Assembly

![line1](media/line1.png)

**Required Parts**

![42_00](media/42_00.png)

![line1](media/line1.png)

**Step 1**

![42_01](media/42_01.png)

![line1](media/line1.png)

**Step 2**

![42_02](media/42_02.png)

![line1](media/line1.png)

**Step 3**

![42_03](media/42_03.png)

![line1](media/line1.png)

**Step 4**

![42_04](media/42_04.png)

![line1](media/line1.png)

**Step 5**

![42_05](media/42_05.png)

![line1](media/line1.png)

**Step 6**

![42_06](media/42_06.png)

![line1](media/line1.png)

**Step 7**

![42_07](media/42_07.png)

![line1](media/line1.png)

**Step 8**

![42_08](media/42_08.png)

![line1](media/line1.png)

**Completed**

![42_09](media/42_09.png)

![line1](media/line1.png)

#### Wiring Diagram

![4202](media/4202.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **4.2Fire alarm.sb3** file.

![4203](media/4203.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Conceive:**

Set a threshold of voltage to determine whether there is flame. When the sensor detects flame, the voltage is lower than the threshold, and the buzzer alarms. The buzzer will stop alarming when the voltage exceeds the threshold (the sensor detects no flame).

![line2](media/line2.png)

**Code structure:**

1. Initialization. Set the pins of the flame sensor and the passive buzzer, set the voltage value of a single scale, and set the frequency of the passive buzzer.

   ![3603](media/3603.png)

2. Loop.

   Print the analog value and voltage of the flame sensor.

   Determine whether the voltage is lower than 4 (<span style="color: rgb(10, 10, 200);">Herein, we set 4 as the threshold, which is adjustable according to needs</span>).

   - voltage < 4: buzzer alarms.
   - voltage ≥ 4: buzzer does not emit sounds.
   
   ![4204](media/4204.png)

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

Upload the code. When the flame sensor detects flame, the voltage will lower than 4, and the buzzer will alarm. If not, the buzzer will not emit sounds.

![4205](media/4205.gif)

![4bottom](media/4bottom.png)

---

### 4.3 Magnetic Field Detection

After the lightning strike, a certain amount of electricity will generated in the surrounding, and a strong magnetic field will be produced in an instant. 

This magnetic field interferes with the connection of the relevant equipment of the station, thus disabling the automatic devices. Therefore, it is necessary to detect the magnetic field at all times and alarm immediately when the magnetic field is detected.

In this experiment, we utilize a Hall sensor and a white LED module to detect magnetic field. When the Hall sensor detects a magnetic field, the white LED lights up.

#### Flow

![4301](media/4301.png)

#### Assembly

![line1](media/line1.png)

**Required Parts**

![43_00](media/43_00.png)

![line1](media/line1.png)

**Step 1**

![43_01](media/43_01.png)

![line1](media/line1.png)

**Step 2**

![43_02](media/43_02.png)

![line1](media/line1.png)

**Step 3**

![43_03](media/43_03.png)

![line1](media/line1.png)

**Step 4**

![43_04](media/43_04.png)

![line1](media/line1.png)

**Step 5**

![43_05](media/43_05.png)

![line1](media/line1.png)

**Step 6**

![43_06](media/43_06.png)

![line1](media/line1.png)

**Step 7**

![43_07](media/43_07.png)

![line1](media/line1.png)

**Completed**

![43_08](media/43_08.png)

![line1](media/line1.png)

#### Wiring Diagram

![4302](media/4302.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **4.3Magnetic field detection.sb3** file.

![4303](media/4303.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Conceive:**

When the Hall sensor detects a magnetic field, a low power(0) will be output, and the white LED lights up. If there is no magnetic field, high(1) will be output, and the LED goes off.

![line2](media/line2.png)

**Code structure:**

1. Initialization. Set the pins of the Hall sensor and the white LED module.

   ![4304](media/4304.png)

2. Loop.

   Print the digital value of the power level of the Hall sensor.

   Determine whether the value equals 0 (0 means a magnetic field is detected). 

   - value = 0: the white LED lights up.
   - value ≠ 0: the white LED goes off.

   ![4305](media/4305.png)


![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

After uploading the code, the Hall sensor starts to detect magnetic field.

If the sensor detects a magnetic field, the white LED will turn on. If not, the LED will go off.

![4306](media/4306.gif)

![4bottom](media/4bottom.png)

---

### 4.4 Thunder Detection

Thunder is the atmospheric sound produced by lightning. When thunder is detected, it sends an alert that rain may be coming.

In this experiment, we integrate a sound sensor and a white LED module to construct a thunder detector. When the thunder volume exceeds a set threshold, the white LED will lights up.

#### Flow

![4401](media/4401.png)

#### Assembly

![line1](media/line1.png)

**Required Parts**

![44_00](media/44_00.png)

![line1](media/line1.png)

**Step 1**

![44_01](media/44_01.png)

![line1](media/line1.png)

**Step 2**

![44_02](media/44_02.png)

![line1](media/line1.png)

**Step 3**

![44_03](media/44_03.png)

![line1](media/line1.png)

**Step 4**

![44_04](media/44_04.png)

![line1](media/line1.png)

**Step 5**

![44_05](media/44_05.png)

![line1](media/line1.png)

**Step 6**

![44_06](media/44_06.png)

![line1](media/line1.png)

**Step 7**

![44_07](media/44_07.png)

![line1](media/line1.png)

**Completed**

![44_08](media/44_08.png)

![line1](media/line1.png)

#### Wiring Diagram

![4402](media/4402.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **4.4Sound detection.sb3** file.

![4403](media/4403.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Conceive:**

Set a threshold of analog value to determine the thunder volume. When thunder is detected, the analog value exceeds the threshold, and the white LED lights up as an alarm. The LED will go off when the value is lower than the threshold.

![line2](media/line2.png)

**Code structure:**

1. Initialization. Set the pins of the sound sensor and the white LED module.

   ![4404](media/4404.png)

2. Loop.

   Print the analog value of sound volume detected by the sound sensor.

   Determine whether the analog value is greater than 100 (<span style="color: rgb(10, 10, 200);">Herein, we set 100 as the standard threshold of thunder volume, which is adjustable according to needs</span>).

   - analog value > 100, the white LED lights up.
   - analog value ≤ 100, the white LED goes off.
   
   ![4405](media/4405.png)

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

After uploading the code, the sound sensor detects whether there is a thunder. When the analog value of the sound exceeds 100, a thunder is detected and the white LED will light up.

Here we stimulate thunder by playing music. When the value is greater than 100, LED lights up.

![4406](media/4406.gif)

![4bottom](media/4bottom.png)

---

### 4.5 Temperature Detection

It is necessary to monitor the atmospheric temperature in the natural environment in real time. If the temperature is too high, disasters such as fire may occur. When the normal temperature is detected, the green LED lights up; the yellow LED is a reminder for raising temperature; if red LED is on, be very careful because it indicates a high temperature!

In this experiment, the XHT11 temperature and humidity sensor and the traffic light module to measure temperature range. Three colors of LED indicate three ranges of ambient temperature. 

#### Flow

![4501](media/4501.png)

#### Assembly

![line1](media/line1.png)

**Required Parts**

![45_00](media/45_00.png)

![line1](media/line1.png)

**Step 1**

![45_01](media/45_01.png)

![line1](media/line1.png)

**Step 2**

![45_02](media/45_02.png)

![line1](media/line1.png)

**Step 3**

![45_03](media/45_03.png)

![line1](media/line1.png)

**Step 4**

![45_04](media/45_04.png)

![line1](media/line1.png)

**Step 5**

![45_05](media/45_05.png)

![line1](media/line1.png)

**Step 6**

![45_06](media/45_06.png)

![line1](media/line1.png)

**Completed**

![45_07](media/45_07.png)

![line1](media/line1.png)

#### Wiring Diagram

![4502](media/4502.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **4.5Temperature detection.sb3** file.

![4503](media/4503.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Conceive:**

Set three thresholds to separate the temperature range: 24, 29, 35, which are adjustable according to needs.

- preference temperature: 24°C ~ 29°C
- warning temperature: 29°C ~ 35°C
- high temperature: over 35°C

Corresponding LED will light up when the ambient temperature is within the related ranges.

- Within preference temperature range: the green LED lights up
- Within warning temperature range: the yellow LED lights up.
- Within high temperature range: the red LED lights up.

![line2](media/line2.png)

**Code structure:**

1. Initialization. Set the pins of XHT11 temperature and humidity sensor and the traffic light module.

   ![4504](media/4504.png)

2. Loop.

   XHT11 sensor reads and outputs the temperature values.

   Determine which section the temperature value is in, so then light up corresponding LED.

   - 24°C ≤ temperature < 29°C: the green LED lights up and other LEDs are off.
   - 29°C ≤ temperature < 35°C: the yellow LED lights up and other LEDs are off.
   - temperature > 35°C: the red LED lights up and other LEDs are off.
   
   ![4505](media/4505.png)

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

After uploading the code, the XHT11 sensor detects the ambient temperature value.

When the value is in the preference temperature range, the green LED lights up;

When the value is within the warning temperature range, the yellow LED turns on;

When the value exceeds the high temperature threshold, the red LED lights up.

![4506](media/4506.gif)

![4bottom](media/4bottom.png)

---

### 4.6 Ultraviolet Detection

In daily life, when the UV index is greater than 3, you'd better do sunscreen measures when going out. This station will calculate the UV index in real time to make timely reminders.

In this experiment, we detect the UV index with an ultraviolet sensor and a traffic light module. When the detected UV index is higher than a set threshold, the red LED will light up.

#### Flow

![4601](media/4601.png)

#### Assembly

![line1](media/line1.png)

**Required Parts**

![46_00](media/46_00.png)

![line1](media/line1.png)

**Step 1**

![46_01](media/46_01.png)

![line1](media/line1.png)

**Step 2**

![46_02](media/46_02.png)

![line1](media/line1.png)

**Step 3**

![46_03](media/46_03.png)

![line1](media/line1.png)

**Step 4**

![46_04](media/46_04.png)

![line1](media/line1.png)

**Step 5**

![46_05](media/46_05.png)

![line1](media/line1.png)

**Step 6**

![46_06](media/46_06.png)

![line1](media/line1.png)

**Step 7**

![46_07](media/46_07.png)

![line1](media/line1.png)

**Completed**

![46_08](media/46_08.png)

![line1](media/line1.png)

#### Wiring Diagram

![4602](media/4602.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **4.6Ultraviolet detection.sb3** file.

![4603](media/4603.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Conceive:**

When the UV index is within 0 ~ 2, the ultraviolet light is the weakest, and it does not have much effect on the human body. When the index increases to 3 ~ 4, the ultraviolet light is weak, but remember to wear sunscreen when going out. 

Herein, we set the threshold of the UV index to 3. If the value exceeds 3, the red LED will light up to remind you to wear sunscreen. If the value does not reach 3, the LED will go off.

![line2](media/line2.png)

**Code structure:**

1. Initialization.

   ![4604](media/4604.png)

2. Loop:

   if elif statement to determine the range of UV index, and output the value.

   Determine whether the UV index exceeds 3.

   - UV index > 3: the red LED lights up as a reminder.
   - UV index ≤ 3: the red LED goes off.
   
   ![4605](media/4605.png)

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

After uploading the code, when the UV index is greater than 3, the red LED will light up to remind you to take sun protection measures when going out.

![4606](media/4606.gif)

![4bottom](media/4bottom.png)

---
### 4.7 Air Pressure Detection

The station monitors air pressure in real time. When the air pressure is in normal range, the green LED lights up; When it is in the low range, the yellow LED turns on; When it is high, the red LED is on.

In this experiment, we use an LPS331APTR air pressure sensor and a traffic light module to reveal the air pressure. LED will light up in corresponding colors when the pressure value is in the related set range.

#### Flow

![4701](media/4701.png)

#### Assembly

![line1](media/line1.png)

**Required Parts**

![47_00](media/47_00.png)

![line1](media/line1.png)

**Step 1**

![47_01](media/47_01.png)

![line1](media/line1.png)

**Step 2**

![47_02](media/47_02.png)

![line1](media/line1.png)

**Step 3**

![47_03](media/47_03.png)

![line1](media/line1.png)

**Step 4**

![47_04](media/47_04.png)

![line1](media/line1.png)

**Step 5**

![47_05](media/47_05.png)

![line1](media/line1.png)

**Step 6**

![47_06](media/47_06.png)

![line1](media/line1.png)

**Step 7**

![47_07](media/47_07.png)

![line1](media/line1.png)

**Step 8**

![47_08](media/47_08.png)

![line1](media/line1.png)

**Step 9**

![47_09](media/47_09.png)

![line1](media/line1.png)

**Completed**

![47_10](media/47_10.png)

![line1](media/line1.png)

#### Wiring Diagram

![4702](media/4702.png)

#### Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![3111](media/3111.png)

Choose D:\Code\1.Code_kidsuno to open **4.7Air pressure detection.sb3** file.

![4703](media/4703.png)

Click ![Unconnected](media/Unconnected.png)to connect to port and then  ![2210](media/2210.png).

#### Explanations

![5top](media/5top.png)

**Conceive:**

Generally, air pressure within 950hPa ~ 1050hPa is regared as the normal range. If the pressure is lower than 950hPa or higher than 1050hPa, human may have a headache or dizziness, and even some meteorological disasters will happen.

Set 950 and 1050 as two thresholds to divide the pressure into three ranges.

- low pressure: lower than 950hPa
- normal pressure: 950hPa ~ 1050hPa 
- high pressure: higher than 1050hPa

LED will light up in corresponding colors when the pressure value is in the related set range.

- Within low pressure range: the yellow LED lights up.
- Within normal pressure range: the green LED lights up.
- Within high pressure range: the red LED lights up.

![line2](media/line2.png)

**Code structure:**

1. Initialization. set the pins of LPS331APTR air pressure sensor and the traffic light module.

   ![4704](media/4704.png)

2. Loop.

   LPS331APTR sensor reads the air pressure value and outputs it.

   Determine which range of the pressure value is in, in order to turn of related LED.

   - air pressure > 1050hPa: the red LED lights up and other two LEDs goes off.
   - air pressure < 950hPa: the yellow LED lights up and other two LEDs goes off.
   - 950hPa < air pressure < 1050hPa: the green LED lights up and other two LEDs goes off.

   ![4705](media/4705.png)

![5bottom](media/5bottom.png)

#### Test Result

![4top](media/4top.png)

After uploading the code, the LPS331APTR sensor measures the air pressure.

When the air pressure is in normal range, the green LED lights up;

When the air pressure is in the low range, the yellow LED lights up;

When the air pressure is in the high range, the res LED turns on.

![4706](media/4706.gif)

![4bottom](media/4bottom.png)

---

