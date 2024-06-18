# Mini Meteorological Station for kidsuno

## 1. Code

[DOWNLOAD](../Code.zip)

Download and unzip these files. Here all codes are in folder **1.Code_kidsuno**.

For convenience, <span style="color: rgb(2550, 10, 50);">we move the codes into: **D:\Code\1.Code_kidsuno**.</span> You can also choose to move it into any disks at will. 

---

## 2. Development Environment Configuration

2.1 KidsBlock Download

![图片不存在](media/5cfd05b93a224faf3652714ae17784aa.png)

1. [KidsBlock Download](https://wiki.kidsbits.cc/projects/KidsBlock/en/latest/download/)
2. Installation
	- [Windows System](https://wiki.kidsbits.cc/projects/KidsBlock/en/latest/Windows/)
	- [MacOS System](https://wiki.kidsbits.cc/projects/KidsBlock/en/latest/MacOS/)
3. [Driver Installation](https://wiki.kidsbits.cc/projects/KidsBlock/en/latest/driver/)

---

2.2 KidsBlock Tutorial

1. Make sure the board is connected to computer. Open KidsBlock and choose a device.

![图片不存在](media/c934c531b2f1f69ecdc2d084f5e14cea.png)

Choose **kidsuno**.

![图片不存在](media/045ad281bace3d7c01190b99c0b945f1.png)

Click **Connect**.

![图片不存在](media/bc8f0b2502e5338da3485b694d27777f.png)

**Go to Editor**.

![图片不存在](media/24a80c33bf61182e2903ce972f303edf.png)

Click ![图片不存在](media/b9f32f062d03d5ae9e938220016c577d.png) to switch to upload mode.

![图片不存在](media/a9227e694968e46b62858ae4aaab5185.png)

![图片不存在](media/d8ff78daa5e990bf996d106966d418f7.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

2. Build code blocks and upload.

**Method ①**: Directly drag blocks to the editing area.

![图片不存在](media/50044e4f0feeeba139c639a071a4c25b.png)

After building your blocks, save it to your computer: **File --> Save to your computer**

![图片不存在](media/7a56aca6cd4a0ac536c58fb6508ae4cd.png)

Click ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png) to upload the code.

![图片不存在](media/5ec63b60c74ec72ce8ed8604616cc20f.png)

**Method ②**: Load code from your computer.

Download code in **1. Code** to your computer. For convenience, here we save it to D:\Code\1.Code_kidsuno.

**File --> Load from your computer** and choose code to open.

![图片不存在](media/7a56aca6cd4a0ac536c58fb6508ae4cd.png)

After loading code, connect to the corresponding port.

![图片不存在](media/5e9f0159b548e3b704080791ce61076d.png)

![图片不存在](media/bc8f0b2502e5338da3485b694d27777f.png)

After that, click ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png)to upload code.

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Main Interface**

![图片不存在](media/3852252c8a85875f8f5db8f171258707.png)

![图片不存在](media/f7056bd04a4e2d7b28ebd012b87da16a.png)

---

## 3. Modules

<span style="color: rgb(2550, 10, 50);">Please move the codes to a convenient path as your needs, for instance, path: **D:\Code\1.Code_kidsuno**.</span>

kidsuno Ports View

During experiments, <span style="color: rgb(2550, 10, 50);">modules can only be connected to ports in the same color.</span>

![图片不存在](media/027484a643d090a640ed0ef220ef1310.png)

3.1 White LED Module

![图片不存在](media/0f796489e3fccd806ac608826e78772c.png)

![图片不存在](media/a22119f910ee2e8172fdba2106151e8e.png)

**LED (Light-Emitting Diode)**

LED is a commonly used light emitting device that converts electrical energy into light energy. Usually, it is used as an indicator in circuits and instruments, or as part of texts or numeric display.

It generally includes gallium(Ga), arsenic(As), phosphorus(P), nitrogen(N) and so on. 

|     LED components      | Emitting light colors |
| :---------------------: | :-------------------: |
| gallium arsenide diode  |          red          |
| gallium phosphide diode |         green         |
|  silicon carbide diode  |        yellow         |
|  gallium nitride diode  |         blue          |

![图片不存在](media/574fafd11b0076d3a77d6b35961bec45.png)

Parameters

![图片不存在](media/bb22aeac8f0bbe54abccb1cb3e9a155a.png)

Operating voltage: DC 3.3 ~ 5 V

Operating current: 1.5 mA (Peak: 2.3mA)

Maximum power: 0.07 W

Control signal: digital signal

Dimensions: 24 x 48 x 18 mm (without housing)

Positioning holes: diameter of 4.8 mm

Interface: telephone socket

![图片不存在](media/ff61b588417e98ef8df9e4d9834f8c52.png)

Principle

![图片不存在](media/dda544dbaa39b4e95f3be6d8b44aa584.png)

Modules with blue housing are digital ones, so we should connect to digital io pins of the mainboard (ports with blue).

![图片不存在](media/81c4e4559262115911009c201ec81f4b.png)

In this experiment, we connect the white LED module to port 1. According to the board ports view, the digital io pin at port 1 is D5.

When we set the pin to high(1), the LED lights up in white; if we set to low(0), it will be off.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/9bdc63021a79f46d54c253cdc11170ab.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **3.1Light_on.sb3** file.

![图片不存在](media/81a479595b40bfcdd08fb87c1a285205.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Code Blocks**

|            Blocks             |          Code block           |
| :---------------------------: | :---------------------------: |
|  ![图片不存在](media/b235f1924c2c2c6201df43967b104116.png)  |   ![图片不存在](media/7b373bcabc1aed5fc0b05092679a22fa.png)   |
|       ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)       | ![图片不存在](media/fe7119610b2cdfe715aaaba76dbf0757.png) |
|       ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)       |  ![图片不存在](media/5530574a048b6ebc200f7c7d8d974850.png)  |
| ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png) | ![图片不存在](media/27ff2f64a99f85b0f74de875ad5572ec.png) |
| ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png) |    ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png)    |

![图片不存在](media/58b75ba1ba6bfa524479ef35a58fcf13.png)

**Conceive:**

1. **Initialization**

   Set pins and modes.

   ![图片不存在](media/3b5cc7c84e181386c9f8e55d79517265.png)

   <br>

   **Build blocks:**

   ① Add ![图片不存在](media/7b373bcabc1aed5fc0b05092679a22fa.png) and ![图片不存在](media/fe7119610b2cdfe715aaaba76dbf0757.png) .

   ② Set pin to 5.

   ![图片不存在](media/4b9b24a9448f6151b527c81dfa100232.png)

   ③ set mode to output.

   pin mode can be one of the followings:

   - input
   - output
   - input-pullup

   ![图片不存在](media/2f5f4d9ef54812ea08960cca8a8806e8.png)
   
   Q ：Why "output"?

   A ：<span style="color: rgb(10, 10, 200);">The code is written for the mainboard.</span> For the board, pin D5 is outputting power levels (high or low) to the connected module.

   ![图片不存在](media/bcc144c573b815d3bad3fed954f006c2.png)

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

2. **Main Code**

   Loop: LED turns on for 1s and off for 1s.

   ![图片不存在](media/5492bfb29b51ae464d5a7e64357596c7.png)

   <br>

   **Build blocks:**

   ① Add ![图片不存在](media/27ff2f64a99f85b0f74de875ad5572ec.png) . Code blocks in it will run in a loop.

   ② Put ![图片不存在](media/5530574a048b6ebc200f7c7d8d974850.png) into "forever". 

   This block set output power level:

   - high
   - low
   
   Set pin to 5, and set to output high.

   ③ Add a delay ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png).

   ![图片不存在](media/2f5f4d9ef54812ea08960cca8a8806e8.png)

   Q ：Why delay?

   A ：If you output a high level to LED, it will be always on. Yet, we add a delay of 1s, so it lights up for only 1s. Delay time is the ON/OFF time of LED.

   ![图片不存在](media/bcc144c573b815d3bad3fed954f006c2.png)

   Set pin D5 to output high for 1s:

   ![图片不存在](media/7e10909c2ae891eac3a69e6b58430665.png)

   ④ Duplicate the blocks.

   ![图片不存在](media/46f68e23d4ecef9f71590739e16b4b52.png)

   As follows:

   ![图片不存在](media/07b925242199fc65a4d248fed87ac24a.png)

   Modify to low. Pin D5 outputs low for 1s:

   ![图片不存在](media/ed5f0f4151fe6e4312fea08cbd23ab7a.png)

   The LED will circularly be on for 1s and off for 1s.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading code, the LED module will flash with an interval of 1s (on for 1s and off for 1s).

![图片不存在](media/d60aa95d6e9040d62f3c15db68fb6d66.gif)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

3.2 Hall Magnetic Sensor

![图片不存在](media/0f796489e3fccd806ac608826e78772c.png)

![图片不存在](media/3ca2db2df249fd47e6d58bad1b06d0a9.png)

This Hall sensor module is mainly composed of A3144 linear Hall components. 

Based on Hall Effect, its magnetic sensitive circuit adopts semiconductor integration technology, which is a magnetic sensing circuit composed of a voltage regulator, a Hall voltage generator, a differential amplifier, a Schmidt trigger temperature compensation circuit and an open-collector output stage. 

Its input is the magnetic induction intensity and its output is a digital voltage signal.

![图片不存在](media/574fafd11b0076d3a77d6b35961bec45.png)

Parameters

![图片不存在](media/bb22aeac8f0bbe54abccb1cb3e9a155a.png)

Voltage: DC 3.3 ~ 5V 

Current: 10 mA

Maximum power: 0.05 W

Operating temperature: -10°C ~ +50°C

Dimensions: 32 x 24 x 18 mm (without housing)

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![图片不存在](media/ff61b588417e98ef8df9e4d9834f8c52.png)

Principle

![图片不存在](media/dda544dbaa39b4e95f3be6d8b44aa584.png)

This Hall sensor is able to distinguish magnetic field north and south. The front of the magnetic induction element (with numbers) senses the South Pole, while its back detects the North Pole.

![图片不存在](media/6aee28639f5ba48880bea0cc37ffd40b.png)

Modules with blue housing are digital ones, so we should connect to digital io pins of the mainboard (ports with blue).

![图片不存在](media/81c4e4559262115911009c201ec81f4b.png)

In this experiment, we connect the Hall sensor module to port 2. According to the board ports view, the digital io pin at port 2 is D6.

When a magnetic field is detected, Hall sensor outputs low; When no magnetic field is detected, the sensor outputs high.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/b29ad7c8149d7c5fbc3f74e80da5a811.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **3.2Hall sensor.sb3** file.

![图片不存在](media/0b15dcd28cb4a99e25d9732221b26827.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Code Blocks**

|              Blocks               |              Code block               |
| :-------------------------------: | :-----------------------------------: |
|    ![图片不存在](media/b235f1924c2c2c6201df43967b104116.png)    |       ![图片不存在](media/7b373bcabc1aed5fc0b05092679a22fa.png)       |
|         ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)         |     ![图片不存在](media/fe7119610b2cdfe715aaaba76dbf0757.png)     |
|         ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)         | ![图片不存在](media/4a476f8c2b33d23566173c704b881aa9.png) |
|    ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)    | ![图片不存在](media/16dd3f0662036ce7fad5168fd63271dc.png) |
|    ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)    | ![图片不存在](media/d4d3e61093e6004a1eb76439a8c6e47b.png) |
| ![图片不存在](media/193782c9c20d945ae0208e5327d6697d.png) |           ![图片不存在](media/39d9ee5719271fed28fe37212feb6b49.png)           |
|   ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)   |     ![图片不存在](media/27ff2f64a99f85b0f74de875ad5572ec.png)     |
|   ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)   |      ![图片不存在](media/b2c84d5fb7db813965d4c1f256305faf.png)      |
|   ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)   |        ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png)        |

![图片不存在](media/58b75ba1ba6bfa524479ef35a58fcf13.png)

**Conceive:**

1. **Initialization**

   Set pins and modes, initialize serial port.

   ![图片不存在](media/5dd7139bc5ab3dc3112cd6b4b40a897a.png)

   <br>

   **Build blocks:**

      ① Drag blocks and build as follows:

   ![图片不存在](media/cda17642ff0320ffa6b369e8cab4b0b9.png)

   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)

      ![图片不存在](media/16dd3f0662036ce7fad5168fd63271dc.png) : initialize serial port. Set baud rate (9600 by default). This block is indeed if you need to display messages on serial monitor. Otherwise, it fails to output.

   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)

   Connect Hall sensor to pin D6 on the board, and set it to input.

   ![图片不存在](media/2f5f4d9ef54812ea08960cca8a8806e8.png)

   Q ：Why "input"?

   A ：<span style="color: rgb(10, 10, 200);">The code is written for the mainboard.</span> For the Hall sensor, it is outputting power levels to the pin D6 on the board, so the board is receiving(inputting) levels.

   ![图片不存在](media/bcc144c573b815d3bad3fed954f006c2.png)

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

2. **Main Code**

   Loop: If a magnetic field is detected, serial monitor prints *A magnetic field*. If not, it displays *There is no magnetic field*.

   ![图片不存在](media/047d6a88c9e67fef8150b278a32a4198.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![图片不存在](media/0e0fea6bd791b28aa2e5a7d3fd5c4d1d.png)

   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)

   ![图片不存在](media/4a476f8c2b33d23566173c704b881aa9.png) reads digital power levels and outputs 1(high) or 0(low).

   ![图片不存在](media/d4d3e61093e6004a1eb76439a8c6e47b.png) will prints the messages in it on the serial monitor. Or you can put some variables in the printing box to display their values. Three modes are available: wrap, no wrap, HEX.

   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)

   Set pin to D6 and print the value without wrapping.

   ![图片不存在](media/27ed0f416b2ffe10d5e6f7358ed1423d.png)

   ![图片不存在](media/2f5f4d9ef54812ea08960cca8a8806e8.png)

      Q ：Why no-wrap?

      If we set to wrap, the message will have a line break after the power level value being output.

      Wrap: 

      ![图片不存在](media/6ed5905a989d615100a966af9e621960.png)

      No-wrap:

      ![图片不存在](media/6fb6b64cdcb0d8a224e43a6d5a8675f6.png)

      A ：No-wrap is more convenient for us to check the results.

   ![图片不存在](media/bcc144c573b815d3bad3fed954f006c2.png)

   ② Drag blocks and build as follows:

   ![图片不存在](media/eaa3e2794ef7bba2de0a326c0cc31fb9.png)

   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)

   ![图片不存在](media/39d9ee5719271fed28fe37212feb6b49.png): check whether the two values equal each other. If yes, outputs true.

   ![图片不存在](media/b2c84d5fb7db813965d4c1f256305faf.png): if else. It determines the condition is true or false. 

   True: execute codes in "if":

   ![图片不存在](media/2f76c55ac91ea5fbbdf7a0c93a08d094.png)

   False: execute codes in "else":

   ![图片不存在](media/dfb37008280a9ba4068bc97223e6ba14.png)

   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)

   ![图片不存在](media/fe8e4e653ccb8888817260c98aed4a45.png) determines whether the value read by pin D6 equals 0. Put it in "if else" block to set it to the condition.

   value of pin D6 = 0: the condition is true, execute codes in "if", and print two Space + *A magnetic field* on the serial monitor.

   value of pin D6 ≠ 0: the condition is false, execute codes in "else", and print two Space + *There is no magnetic field* .

   ![图片不存在](media/2f5f4d9ef54812ea08960cca8a8806e8.png)

      Q ：Why Space?

   The value will be too close to the contents, which is not convenient for us to check the outputs.

   Without space:

      ![图片不存在](media/2a0efd4258a3e51962bf6bae154f2032.png)

     With space:

      ![图片不存在](media/85b49a5db293b1b8b94aafeaed369510.png)

      A ：We add a space to separate the value and contents.

   ![图片不存在](media/bcc144c573b815d3bad3fed954f006c2.png)

   ③ Add a delay ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png) and set the time to 0.1s.

   ![图片不存在](media/2f5f4d9ef54812ea08960cca8a8806e8.png)

   Q ：Why delay?

   If we do not add a delay, the printing command will always run, so then the serial monitor refreshes the results very fast. A delay of 0.1s will limit the printing speed. Serial monitor refreshes outputs every 0.1s.

   A ：Limit the printing speed.

   ![图片不存在](media/bcc144c573b815d3bad3fed954f006c2.png)


![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![图片不存在](media/81687183903f3a617cf2f7088b089c33.png) and set Buadrate to 9600.

![图片不存在](media/6d861659d1bb976ce0da011cb5a31997.png)

After uploading the code, when the **South Pole** of the magnet approaches to the front of the magnetic induction element, the red LED lights up and Shell prints *0  A magnetic field*; 

![图片不存在](media/c0741f51c46a8a5e6f438d87bc5de92b.png)

When the **South Pole** of the magnet approaches to its back or is away from the sensor, the red LED goes off, and Shell prints *1  There is no magnetic field* .

![图片不存在](media/4afb5ba7145d0fdc2462f3e86d6c4928.png)

Put the **North Pole** of the magnet to the back of the element, the red LED lights up and Shell prints *0  A magnetic field*; 

![图片不存在](media/2cfffb7160fc70c2f1243b59c1dc6ccf.png)

When the **North Pole** of the magnet approaches to the front of the sensor or is away from it, the red LED goes off, and Shell prints *1  There is no magnetic field*.

![图片不存在](media/9d826c2ebf795347d3d574cc08af4b5e.png)

![图片不存在](media/4f3488d96ba192e7994227c4504971a2.gif)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

3.3 Passive Buzzer

![图片不存在](media/0f796489e3fccd806ac608826e78772c.png)

![图片不存在](media/ff3d76372cb787a611199a128dc13303.png)

Buzzer is an integrated structure of electronic sound device, which is powered by DC voltage. In application, it is widely used in computers, printers, copiers, alarms, electronic toys, automotive electronic equipment, telephones and timers. 

Buzzers can be divided into active ones(built-in drive circuits) and passive ones(external drive) according to that whether they includes an excitation source.

Active buzzers contain oscillation source inside, which can sound at a fixed frequency once be triggered. They are convenient in program control and features high sound pressure.

Passive ones, however, do not include oscillating sources. If we directly power a passive buzzer via DC voltage, it will emit no sound. According to needs, we generally drive through square waves, whose frequency determines the sound tones.

**To sum up, The active buzzer contains a vibration source, and its sound frequency is fixed. Yet there is no vibration source inside the passive one, so it must be driven by square waves whose frequency can be changed to control sounds.**

![图片不存在](media/574fafd11b0076d3a77d6b35961bec45.png)

Parameters

![图片不存在](media/bb22aeac8f0bbe54abccb1cb3e9a155a.png)

Operating voltage: DC 3.3 ~ 5V 

Operating temperature: -10°C ~ +50°C

Control signal: Digital signal

Dimensions: 48 x 24 x 18 mm (without housing)

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![图片不存在](media/ff61b588417e98ef8df9e4d9834f8c52.png)

Principle

![图片不存在](media/dda544dbaa39b4e95f3be6d8b44aa584.png)

Music is an invisible art. It is a language that narrates emotions and thoughts. 

The foundation of music, as we all know, is note. We can compose a variety of melodies and rhythms with different notes. Of all the notes, the most basic are seven:

![图片不存在](media/66e6823bf861f8cad52bc0611ca9d997.png)

We can compose a variety of melodies and rhythms with these notes.

Passive buzzer module must be drive by square waves to emit sound. We can change the duty cycle of PWM to control square waves.

- The greater the duty cycle is, the lauder the sound will be.

And the tones vary from different frequency of PWM.

- The higher the frequency is, the higher the tone will be.

![图片不存在](media/2fd65b883dd17bd50a77af9b5bdb37c2.png)

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

**What is PWM?**

PWM (Pulse width modulation) simulates the change of analog signal through digital signal.

Pulse width is the high level in a complete square wave cycle. So, pulse width modulation is to adjust the high level(of course, in other words, low level is also adjusted).

![图片不存在](media/5b8b29a16e235513a47e4519cd8e8a86.png)

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
	
	![图片不存在](media/89e6481176c78795322869df5feff457.gif)
	
	<center>The relationship between duty cycle and LED brightness<center>

The longer the high level time is, the greater the duty cycle will be, and the brighter the LED will be.

**The PWM frequency corresponding to notes**:

![图片不存在](media/bd6f281865cd802b82db6bc86bbe502f.png)

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

Modules with blue housing are digital ones, so we should connect to digital io pins of the mainboard (ports with blue).

![图片不存在](media/81c4e4559262115911009c201ec81f4b.png)

In this experiment, we connect the passive buzzer to port 3. According to the board ports view, the digital io pin at port 3 is D3.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/742335e4aaac0f8e82b5ee3f902fc446.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **3.3Passive buzzer.sb3** file.

![图片不存在](media/f32c1031620198aa505043c6a90b29cb.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Code Blocks**

|            Blocks             |              Code block               |
| :---------------------------: | :-----------------------------------: |
|  ![图片不存在](media/b235f1924c2c2c6201df43967b104116.png)  |       ![图片不存在](media/7b373bcabc1aed5fc0b05092679a22fa.png)       |
|  ![图片不存在](media/f16caa0686c3a27124959fa8b1cf950a.png)  | ![图片不存在](media/f68c51ddb7e49ecd54e163189413e0d6.png) |
| ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png) |     ![图片不存在](media/27ff2f64a99f85b0f74de875ad5572ec.png)     |
| ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png) |        ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png)        |

![图片不存在](media/58b75ba1ba6bfa524479ef35a58fcf13.png)

**Conceive:**

Add library first. Click ![图片不存在](media/62c05ffc94b8065d1e8be8dbf5956696.png) and find **Passive buzzer** to add in extension.

![图片不存在](media/cca0358197d2a4aa959b625c2e607565.png)

Click  **Back**.

![图片不存在](media/a39b356ed32a62bd9d0800bca65a68df.png)

Successfully load.

![图片不存在](media/435915259df72bdfaded2d5f6ab5285c.png)

**Main Code**

Loop: play tones of C, D, E, F, G, A, B, each tone plays 200ms.

![图片不存在](media/d1927d2e48956eab86b58134e5691007.png)

<br>

**Build blocks:**

① Build blocks as follows:

![图片不存在](media/6bd937cccc205874bc7894a9ad0d83d1.png)

Set pin to 3 and frequency to NOTE_C5, add a delay of 0.2s.

![图片不存在](media/44145270ee93755112c0b01426d76bff.png)

② Duplicate this block.

![图片不存在](media/1215143f2f5e670b969faa3b0a68cd35.png)

As follows:

![图片不存在](media/1ee89064a98cb1c1d625a6e7292468ae.png)

Duplicate six times, as follows:

![图片不存在](media/c37917335bfba20951b9f29cbad52c20.png)

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, the buzzer will circularly play tones(C, D ,E, F, G, A, B).

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

Extension

![图片不存在](media/20165af751e3a46de15eb7992240aeba.png)

Congratulations! You have played these basic notes successfully! Now let's try to compose a beautiful music and play with this passive buzzer!

Open **3.3Music.sb3** file.

![图片不存在](media/a82a698aa6e8ce42a27f29c00d0aa4de.png)

Choose a music you like.

![图片不存在](media/07c925adf2992dfc154ffe1e7070f0b0.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Upload! And you will hear the music!

![图片不存在](media/d33d7d83d36b8c3f5effdcdf73bd6f4c.gif)

![图片不存在](media/adb2dc68eebff18cfe59251042f7d5a1.png)


---

3.4 XHT11 Temperature and Humidity Sensor

![图片不存在](media/0f796489e3fccd806ac608826e78772c.png)

![图片不存在](media/fd4eb242f6a61beabfe6482e45638c92.png)

XHT11 sensor is a low-cost and entry-level temperature and humidity sensor, which consists of a resistive humidity sensor and an NTC temperature sensor. It is designed 4-pin single-row pin and adopts single-wire serial interface, so we just add the appropriate pull-up resistance to read values. Moreover, its signal transmission distance can reach more than 20 meters.

![图片不存在](media/574fafd11b0076d3a77d6b35961bec45.png)

Parameters

![图片不存在](media/bb22aeac8f0bbe54abccb1cb3e9a155a.png)

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

![图片不存在](media/ff61b588417e98ef8df9e4d9834f8c52.png)

Principle

![图片不存在](media/dda544dbaa39b4e95f3be6d8b44aa584.png)

Modules with blue housing are digital ones, so we should connect to digital io pins of the mainboard (ports with blue).

![图片不存在](media/81c4e4559262115911009c201ec81f4b.png)

In this experiment, we connect the passive buzzer to port 4. According to the board ports view, the digital io pin at port 4 is D2.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/d7d46f117ebb0382ec31ace3bc7040bf.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **3.4Humiture.sb3** file.

![图片不存在](media/946c3fb28ca1faef0367da8bf9291563.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Code Blocks**

|            Blocks             |              Code block               |
| :---------------------------: | :-----------------------------------: |
|  ![图片不存在](media/b235f1924c2c2c6201df43967b104116.png)  |       ![图片不存在](media/7b373bcabc1aed5fc0b05092679a22fa.png)       |
|  ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)  | ![图片不存在](media/16dd3f0662036ce7fad5168fd63271dc.png) |
|  ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)  | ![图片不存在](media/d4d3e61093e6004a1eb76439a8c6e47b.png) |
|     ![图片不存在](media/7bfdcb87abb53fe8fd1fee04d85d57fc.png)     |     ![图片不存在](media/ae473d7a71f786c74011154322e77a6c.png)     |
|     ![图片不存在](media/7bfdcb87abb53fe8fd1fee04d85d57fc.png)     |       ![图片不存在](media/ad76844701a364938492502626b76bcb.png)       |
|     ![图片不存在](media/7bfdcb87abb53fe8fd1fee04d85d57fc.png)     |       ![图片不存在](media/1e620d261275fddd9a1fb0756040782a.png)       |
| ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png) |     ![图片不存在](media/27ff2f64a99f85b0f74de875ad5572ec.png)     |
| ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png) |        ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png)        |

![图片不存在](media/58b75ba1ba6bfa524479ef35a58fcf13.png)

**Conceive:**

Add library first. Click ![图片不存在](media/62c05ffc94b8065d1e8be8dbf5956696.png) to load **DHT sensor** .

![图片不存在](media/61b3f2d383237a0a997d4f33b4d9e17d.png)


1. **Initialization**

   Initialize serial port to prepare for the display of temperature and humidity value.

   ![图片不存在](media/b4460fd7ca7463bb5ab30066e9302b77.png)

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

2. **Main Code**

   Loop: read and print the temperature and humidity value every 0.5s.

   ![图片不存在](media/78b93b958f270e0c9a13e4f2dd1eb681.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![图片不存在](media/d369d8a9e52030a0f6c2c605d71af70f.png)

   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)

   ![图片不存在](media/ae473d7a71f786c74011154322e77a6c.png) set the sensor pin.

   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)

   ② Drag blocks and build as follows:

   ![图片不存在](media/1974021a094e6956484d282e31a67929.png)

   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)

   ![图片不存在](media/ad76844701a364938492502626b76bcb.png) read the temperature value in the unit of °C or °F.

   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)
   
   Herein, print "temperature:" + measured actual temperature value + " °C" without wrapping. There is a space before °C, which is convenience for us to check results.
   
   ③ Drag blocks and build as follows:
   
   ![图片不存在](media/8226d9fb5f25e7c92d9a0b428e6eac0d.png)
   
   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)
   
   ![图片不存在](media/1e620d261275fddd9a1fb0756040782a.png) reads the humidity value.
   
   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)
   
   This code prints the actual humidity value in the unit of " %" without wrapping. There is also a space before %. What follows " %" is a line break to print next group of values.
   
   ④ Add a delay ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png) and set it to 0.5, so the results will be refreshed every 0.5s.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![图片不存在](media/81687183903f3a617cf2f7088b089c33.png) and set Buadrate to 9600.

![图片不存在](media/6d861659d1bb976ce0da011cb5a31997.png)

After uploading the code, the serial monitor prints the actual temperature and humidity value every 0.5s.

![图片不存在](media/3be840c15e707ae1ea16529df40eb937.png)

Blow to the XHT11 sensor and you will see both temperature and humidity values rise.

![图片不存在](media/6d5d31a83e559898d281eace04285526.png)

![图片不存在](media/5b12ff14d62bf716490f70fedf2d820c.png)



![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

3.5 Steam Sensor

![图片不存在](media/0f796489e3fccd806ac608826e78772c.png)

![图片不存在](media/f56f375c9ca328175c45e9a17eafe1b7.png)

Unlike the previous modules, the steam sensor is an analog module rather than a digital one.

What is the difference? For digital modules, they only output high(3.3V) or low(0V); while analog ones are able to output or input intermediate voltage values through ADC analog ports on the board.

![图片不存在](media/574fafd11b0076d3a77d6b35961bec45.png)

Parameters

![图片不存在](media/bb22aeac8f0bbe54abccb1cb3e9a155a.png)

Operating voltage: DC 3.3 ~ 5V 

Operating current: 1.5 mA

Maximum power: 0.075 W

Operating temperature: -10°C ~ +50°C

Dimensions: 48 x 24 x 18 mm (without housing)

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![图片不存在](media/ff61b588417e98ef8df9e4d9834f8c52.png)

Principle

![图片不存在](media/dda544dbaa39b4e95f3be6d8b44aa584.png)

The steam sensor measures the amount of water through its exposed lines. The water will connect these lines. The more amount of water is, the wider the conductive area will be connected, and the higher the output voltage will be.

With the change of amount of water, the voltage (0 ~ 5V) detected by the analog port will change accordingly. This change is continuous, which means it can be any value within 0 ~ 5V.

<span style="color: rgb(10, 10, 200);">The board can only process digital signals, so we need to convert analog signals in to digital ones. Thus, an ADC(Analog to Digital Converter) acquisition is required.</span>

![图片不存在](media/2fd65b883dd17bd50a77af9b5bdb37c2.png)

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

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

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

Modules with red housing are analog ones, so we should connect to analog io pins of the mainboard (ports with red).

![图片不存在](media/6f2b11cae23d4915dbbd15ec06b222af.png)

In this experiment, we connect the module to port 4. According to the board ports view, the analog io pin at port 4 is A2.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/ff72bc62dc46769c04aacfdb0a8f76d6.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **3.5Steam sensor.sb3** file.

![图片不存在](media/c9d5b79143d2eedf3e04cb9790b8ec0c.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Code Blocks**

|              Blocks               |               Code block                |
| :-------------------------------: | :-------------------------------------: |
|    ![图片不存在](media/b235f1924c2c2c6201df43967b104116.png)    |        ![图片不存在](media/7b373bcabc1aed5fc0b05092679a22fa.png)        |
|         ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)         |      ![图片不存在](media/fe7119610b2cdfe715aaaba76dbf0757.png)      |
|         ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)         |   ![图片不存在](media/2b97f483d6c44ff167f9bcda935a35c1.png)   |
|    ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)    |  ![图片不存在](media/16dd3f0662036ce7fad5168fd63271dc.png)  |
|    ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)    |  ![图片不存在](media/d4d3e61093e6004a1eb76439a8c6e47b.png)  |
|      ![图片不存在](media/8b2ee7d0ec6b1c8e35477bb509b43cab.png)      | ![图片不存在](media/ba7b89221a90fd18f68250051933443d.png) |
|      ![图片不存在](media/8b2ee7d0ec6b1c8e35477bb509b43cab.png)      |  ![图片不存在](media/145808b6b072653f6657c4b48e02eab0.png)  |
|      ![图片不存在](media/8b2ee7d0ec6b1c8e35477bb509b43cab.png)      |     ![图片不存在](media/56cdcbe1ccd5fc9a7555b0be64a7ab61.png)     |
| ![图片不存在](media/193782c9c20d945ae0208e5327d6697d.png) |       ![图片不存在](media/f7242d3975fc80e48eab9d45803f3839.png)       |
| ![图片不存在](media/193782c9c20d945ae0208e5327d6697d.png) |     ![图片不存在](media/d801427f833abd59387b3fea77bd28fd.png)     |
|   ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)   |      ![图片不存在](media/27ff2f64a99f85b0f74de875ad5572ec.png)      |
|   ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)   |         ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png)         |

![图片不存在](media/58b75ba1ba6bfa524479ef35a58fcf13.png)

**Conceive:**

1. **Initialization**

   Set pins and modes, initialize the serial port. Create a variable to store the analog value of steam sensor.

   ![图片不存在](media/1db81d644f9cf1028599bc93d933a792.png)
   
   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)
   
   ![图片不存在](media/ba7b89221a90fd18f68250051933443d.png) defines parameters of a variable.
   
   - ![图片不存在](media/99f5d0cec1b94a35a04dc316d6af15ae.png)
   
     Define a global or local variable.
   
   - ![图片不存在](media/3e460de70b45945d18f97b0967a11e4d.png)
   
     Define the variable type.
   
   - ![图片不存在](media/fd25ef0dae9ff0b7897cbe045a7903c4.png)
   
     Name the variable.
   
   - ![图片不存在](media/4496ff09be49be551851804f43e2d048.png)
   
     Assign an initial value to the variable.
   
   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)
   
   ![图片不存在](media/61790337573d2797b1fe1c9c9a408f8e.png)
   
   Create a float variable named *Water_value* to store the analog value read by the steam sensor, and assign an initial value of 0 to it.

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

2. **Main Code**

   Loop: print the analog value read by the sensor and the voltage converted from the analog value. The results will be refreshed every 0.1s.

   ![图片不存在](media/169cfd979aab2d3566d862ae3889b3d5.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![图片不存在](media/ee2a2b11e5c5d85ffdbfbe9a670e615a.png)
   
   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)
   
   ![图片不存在](media/145808b6b072653f6657c4b48e02eab0.png) sets variable and assigns value to it.
   
   ![图片不存在](media/2b97f483d6c44ff167f9bcda935a35c1.png) reads analog values.
   
   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)
   
   Connect steam sensor to pin A2; Read the value of pin A2 and assign it to *Water_value*.
   
   ② Drag blocks and build as follows:
   
   ![图片不存在](media/1c57129c7ae0b33e6eff7df5330d63a2.png)
   
   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)
   
   ![图片不存在](media/56cdcbe1ccd5fc9a7555b0be64a7ab61.png) represents the variable. 
   
   ![图片不存在](media/d801427f833abd59387b3fea77bd28fd.png) : the two value will be multiplied. It outputs the result.
   
   ![图片不存在](media/f7242d3975fc80e48eab9d45803f3839.png) : the left value will divide by the right value. It outputs the result.
   
   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)
   
   The calculation of actual voltage value:
   
   ![图片不存在](media/c1ce87ec53982474720634d9346bdd85.png)
   
   The output value will be a input voltage value in the unit of V.
   
   ③ Add a delay ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png) and set it to 0.1s. The results will be refreshed every 0.1s.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![图片不存在](media/81687183903f3a617cf2f7088b089c33.png) and set Buadrate to 9600.

![图片不存在](media/6d861659d1bb976ce0da011cb5a31997.png)

After uploading the code, the monitor outputs the detected analog values of water/vapor and the converted voltage values.

![图片不存在](media/7e7bc30f7ac7f501fbce6b75c8ca98ec.png)

The more the amount of water is / the wetter the air is, the greater the analog and voltage value will be.

![图片不存在](media/d9ff7ed5cef26927e70b130a26721c17.png)

Breath on the detection area, or touch it with a wet tissue, and you will see the analog value ans voltage will both increase.

<span style="color: rgb(2550, 10, 50);">**ATTENTION: Be careful when using water, please do not to drip to any other place outside the detection area to aviod a short circuit.**</span>

![图片不存在](media/96d3c13670c8a8558426709f35e6a4a9.png)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

 3.6 Flame Sensor

![图片不存在](media/0f796489e3fccd806ac608826e78772c.png)

![图片不存在](media/163859fbb024658a42cf80b14a16cd05.png)

Since a far-infrared flame probe is reserved, the flame sensor is particularly sensitive to the flame spectrum, so this sensor is an essential part of the fire-fighting robot to find the fire source.

![图片不存在](media/574fafd11b0076d3a77d6b35961bec45.png)

Parameters

![图片不存在](media/bb22aeac8f0bbe54abccb1cb3e9a155a.png)

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

![图片不存在](media/ff61b588417e98ef8df9e4d9834f8c52.png)

Principle

![图片不存在](media/dda544dbaa39b4e95f3be6d8b44aa584.png)

The sensitive element of the sensor is a special infrared receiving diode, which is very sensitive to the infrared generated by the flame. It detects flame by converting the brightness of the flame into power level signals.

Modules with red housing are analog ones, so we should connect to analog io pins of the mainboard (ports with red).

![图片不存在](media/6f2b11cae23d4915dbbd15ec06b222af.png)

In this experiment, we connect the module to port 6. According to the board ports view, the analog io pin at port 6 is A1.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/fe76832a2959ea15cdba7be91763589e.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **3.6Flame sensor.sb3** file.

![图片不存在](media/0068e19d24beddd6c87dc5af3b9fe825.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Code Blocks**

|              Blocks               |               Code block                |
| :-------------------------------: | :-------------------------------------: |
|    ![图片不存在](media/b235f1924c2c2c6201df43967b104116.png)    |        ![图片不存在](media/7b373bcabc1aed5fc0b05092679a22fa.png)        |
|         ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)         |      ![图片不存在](media/fe7119610b2cdfe715aaaba76dbf0757.png)      |
|         ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)         |   ![图片不存在](media/2b97f483d6c44ff167f9bcda935a35c1.png)   |
|      ![图片不存在](media/8b2ee7d0ec6b1c8e35477bb509b43cab.png)      | ![图片不存在](media/ba7b89221a90fd18f68250051933443d.png) |
|      ![图片不存在](media/8b2ee7d0ec6b1c8e35477bb509b43cab.png)      |  ![图片不存在](media/145808b6b072653f6657c4b48e02eab0.png)  |
|      ![图片不存在](media/8b2ee7d0ec6b1c8e35477bb509b43cab.png)      |     ![图片不存在](media/56cdcbe1ccd5fc9a7555b0be64a7ab61.png)     |
|    ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)    |  ![图片不存在](media/16dd3f0662036ce7fad5168fd63271dc.png)  |
|    ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)    |  ![图片不存在](media/d4d3e61093e6004a1eb76439a8c6e47b.png)  |
| ![图片不存在](media/193782c9c20d945ae0208e5327d6697d.png) |       ![图片不存在](media/f7242d3975fc80e48eab9d45803f3839.png)       |
| ![图片不存在](media/193782c9c20d945ae0208e5327d6697d.png) |     ![图片不存在](media/d801427f833abd59387b3fea77bd28fd.png)     |
| ![图片不存在](media/193782c9c20d945ae0208e5327d6697d.png) |         ![图片不存在](media/25295ea6e954d3db107b46f8e315440e.png)         |
|   ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)   |      ![图片不存在](media/27ff2f64a99f85b0f74de875ad5572ec.png)      |
|   ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)   |       ![图片不存在](media/b2c84d5fb7db813965d4c1f256305faf.png)       |
|   ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)   |         ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png)         |

![图片不存在](media/58b75ba1ba6bfa524479ef35a58fcf13.png)

**Conceive:**

1. **Initialization**

   Set pins and modes, initialize the serial port and create variables.

   ![图片不存在](media/5ec9135e4041d749920c4aeaf3154358.png)

   ![图片不存在](media/386550fed7f387ca26d61619d17ab36c.png)

   Create a float variable named *Flame_value* to store the analog value of the flame sensor, assign an initial value of 0.

   ![图片不存在](media/7e56ddbd93148eca432b2e0dcbae1f10.png)

   Create a float variable named *Voltage* to store the actual voltage value, assign an initial value of 0.


![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

2. **Main Code**

   Loop: print the analog value read by the sensor and the voltage converted from the analog value. The results will be refreshed every 0.1s.

   ![图片不存在](media/d9a2f7c3787e0177de37fed1e54b0382.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![图片不存在](media/fa409427faac8e64dc271ae03d7e9bd3.png)

   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)

   ![图片不存在](media/145808b6b072653f6657c4b48e02eab0.png) set variable and assign to it.

   ![图片不存在](media/56cdcbe1ccd5fc9a7555b0be64a7ab61.png) is a variable block.

   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)

   Connect the flame sensor to pin A1, read the analog value of pin A1 and assign it to the variable *Flame_value*. 

   Calculate the actual voltage value and assign it to *Voltage*.

   ② Drag blocks and build as follows:

   ![图片不存在](media/6abe602d4b1ef9f8595a68218124fb46.png)

   Output the analog value and voltage value of the flame sensor.

   ③ Drag blocks and build as follows:

   ![图片不存在](media/32b4e33b087da644bdfe508acd09588b.png)

   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)
   
   ![图片不存在](media/25295ea6e954d3db107b46f8e315440e.png) determines whether left value of less than the right one. If yes, the condition will be output true.
   
   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)
   
   When flame is detected, the voltage decrease. The brighter the flame is, the lower the voltage will be output. 
   
   In this experiment, we set the threshold voltage value to 4 (you can modify this value according to needs), so when the voltage is lower than 4, the flame is detected.
   
   We add an **if else** block to determine whether the voltage output is lower than 4. The voltage is a float value so it is more accurate.
   
   If voltage < 4, the serial monitor will display *Flame detected!* ; When voltage ≥ 4, it will prints *Nothing* .
   
   ④ Add a delay ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png) and set it to 0.1. The results will be refreshed every 0.1s.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![图片不存在](media/81687183903f3a617cf2f7088b089c33.png) and set Buadrate to 9600.

![图片不存在](media/6d861659d1bb976ce0da011cb5a31997.png)

After uploading the code, *Flame detected!* will be displayed on the serial monitor when the flame sensor detects flame.

If no flame is detected, the serial monitor shows *Nothing*.

![图片不存在](media/f5e5d7c79148b4d7e2aa88c8c7c0dac0.png)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

3.7 Sound Sensor

![图片不存在](media/0f796489e3fccd806ac608826e78772c.png)

![图片不存在](media/8ee457d4aeaba05f80b35989dfb7e84f.png)

The sound sensor acts as a microphone that can capture sound information in the environment.

It is consists of a sensitive capacitor microphone for detecting sound and an amplification circuit. It works based on the propagation and vibration of sound. When sound travels near the sensor, the sound wave causes the sensor to vibrate. Then, the sensor converts sound vibrations into electrical signals and sends them for further processing or analysis.

![图片不存在](media/574fafd11b0076d3a77d6b35961bec45.png)

Parameters

![图片不存在](media/bb22aeac8f0bbe54abccb1cb3e9a155a.png)

Operating voltage: DC 3.3 ~ 5V 

Current: 15 mA

Maximum power: 0.075 W

Operating temperature: -10°C ~ +50°C

Dimensions: 48 x 24 x 18 mm

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![图片不存在](media/ff61b588417e98ef8df9e4d9834f8c52.png)

Principle

![图片不存在](media/dda544dbaa39b4e95f3be6d8b44aa584.png)

When you speak loudly or play music to the MIC, these sound signals are converted into electrical ones, which are output at analog ports.

The amplifier circuit on the module amplifies the sound detected by the MIC. We can adjust the amplification by rotating the potentiometer. It is the maximum when we adjust the potentiometer clockwise to the end.

![图片不存在](media/f5b03dfc4b076d2e3c7028a8c6319bee.png)

Modules with red housing are analog ones, so we should connect to analog io pins of the mainboard (ports with red).

![图片不存在](media/6f2b11cae23d4915dbbd15ec06b222af.png)

In this experiment, we connect the module to port 7. According to the board ports view, the analog io pin at port 7 is A0.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/1dfb2f63d927408f8db1913aeb286a98.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **3.7Sound sensor.sb3** file.

![图片不存在](media/3255618c7adb5a9d3899fec71cdb2366.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Code Blocks**

|            Blocks             |              Code block               |
| :---------------------------: | :-----------------------------------: |
|  ![图片不存在](media/b235f1924c2c2c6201df43967b104116.png)  |       ![图片不存在](media/7b373bcabc1aed5fc0b05092679a22fa.png)       |
|       ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)       |     ![图片不存在](media/fe7119610b2cdfe715aaaba76dbf0757.png)     |
|       ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)       |  ![图片不存在](media/2b97f483d6c44ff167f9bcda935a35c1.png)  |
|  ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)  | ![图片不存在](media/16dd3f0662036ce7fad5168fd63271dc.png) |
|  ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)  | ![图片不存在](media/d4d3e61093e6004a1eb76439a8c6e47b.png) |
| ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png) |     ![图片不存在](media/27ff2f64a99f85b0f74de875ad5572ec.png)     |
| ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png) |        ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png)        |

![图片不存在](media/58b75ba1ba6bfa524479ef35a58fcf13.png)

**Conceive:**

1. **Initialization**

   Set pins and modes, initialize the serial port.

   ![图片不存在](media/c28531f7086a1795b451260fc84cf2a2.png)

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

2. **Main Code**

   Loop: print the analog value read by the sound sensor every 0.1s.

   ![图片不存在](media/7996f9e55d0817358b115cd652c7b1f0.png)

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![图片不存在](media/81687183903f3a617cf2f7088b089c33.png) and set Buadrate to 9600.

![图片不存在](media/6d861659d1bb976ce0da011cb5a31997.png)

After uploading the code, speak to the MIC, and monitor will display the analog value of sound volume that is detected by the sound sensor.

![图片不存在](media/0be7e930000b3c55fe5b2fc7a5526f99.png)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

3.8 Ultraviolet Sensor

![图片不存在](media/0f796489e3fccd806ac608826e78772c.png)

![图片不存在](media/9e43601fc6a14e09dcbde167ba0d3e63.png)

In the solar spectrum, the frequency of ultraviolet is higher than that of visible light, so it is invisible. 

Ultraviolet light can be divided into UVA, UVB, UVC, EUV. Among them, UVA causes tanning; UVB may burn skin due to its shorter wavelength; UVC is normally blocked by the ozone layer. 

Through ultraviolet radiation, the skin will produce more melanin, which is distributed upward into the cuticle of the epidermis to form brown spots. So it is the biggest culprit of skin wrinkles, aging or sagging.

But it's not all bad. When ultraviolet light hits the body, it can promote the synthesis of vitamin D to prevent rickets. Besides, it harbors bactericidal efficacy, so some hospitals disinfect by ultraviolet light. In spite of its benefits, too strong ultraviolet will harm the human body, leading to a skin cancer.

![图片不存在](media/574fafd11b0076d3a77d6b35961bec45.png)

Parameters

![图片不存在](media/bb22aeac8f0bbe54abccb1cb3e9a155a.png)

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

![图片不存在](media/ff61b588417e98ef8df9e4d9834f8c52.png)

Principle

![图片不存在](media/dda544dbaa39b4e95f3be6d8b44aa584.png)

This ultraviolet sensor measures the intensity of ultraviolet light and converts it into electrical outputs.

The relationship between the output voltage of the UV sensor and the UV index:

![图片不存在](media/8774c089ac751540608d4e32732aec09.png)

<center>Comparison Table of Voltage and UV Index</center>

We can have a clearly look of the UV index corresponding to the output voltage. <span style="color: rgb(10, 10, 200);">The voltage is in the unit of mV.</span>

Modules with red housing are analog ones, so we should connect to analog io pins of the mainboard (ports with red).

![图片不存在](media/6f2b11cae23d4915dbbd15ec06b222af.png)

In this experiment, we connect the module to port 8. According to the board ports view, the analog io pin at port 8 is A7.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/909aea37994281cad279048bec33238a.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **3.8Solar ultraviolet sensor.sb3** file.

![图片不存在](media/269fb690952d5716d1b236cc8ad7adf5.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Code Blocks**

|              Blocks               |               Code block                |
| :-------------------------------: | :-------------------------------------: |
|    ![图片不存在](media/b235f1924c2c2c6201df43967b104116.png)    |        ![图片不存在](media/7b373bcabc1aed5fc0b05092679a22fa.png)        |
|         ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)         |      ![图片不存在](media/fe7119610b2cdfe715aaaba76dbf0757.png)      |
|         ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)         |   ![图片不存在](media/2b97f483d6c44ff167f9bcda935a35c1.png)   |
|      ![图片不存在](media/8b2ee7d0ec6b1c8e35477bb509b43cab.png)      | ![图片不存在](media/ba7b89221a90fd18f68250051933443d.png) |
|      ![图片不存在](media/8b2ee7d0ec6b1c8e35477bb509b43cab.png)      |  ![图片不存在](media/145808b6b072653f6657c4b48e02eab0.png)  |
|      ![图片不存在](media/8b2ee7d0ec6b1c8e35477bb509b43cab.png)      |     ![图片不存在](media/56cdcbe1ccd5fc9a7555b0be64a7ab61.png)     |
|    ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)    |  ![图片不存在](media/16dd3f0662036ce7fad5168fd63271dc.png)  |
|    ![图片不存在](media/4d06ebaacec608b138428e0beb2f2c2e.png)    |  ![图片不存在](media/d4d3e61093e6004a1eb76439a8c6e47b.png)  |
| ![图片不存在](media/193782c9c20d945ae0208e5327d6697d.png) |       ![图片不存在](media/f7242d3975fc80e48eab9d45803f3839.png)       |
| ![图片不存在](media/193782c9c20d945ae0208e5327d6697d.png) |     ![图片不存在](media/d801427f833abd59387b3fea77bd28fd.png)     |
| ![图片不存在](media/193782c9c20d945ae0208e5327d6697d.png) |         ![图片不存在](media/25295ea6e954d3db107b46f8e315440e.png)         |
| ![图片不存在](media/193782c9c20d945ae0208e5327d6697d.png) |      ![图片不存在](media/19475c6dc699433b285feba386d1cd74.png)      |
| ![图片不存在](media/193782c9c20d945ae0208e5327d6697d.png) |          ![图片不存在](media/acc07e3e4671abf870f3db5769414e09.png)          |
|   ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)   |      ![图片不存在](media/27ff2f64a99f85b0f74de875ad5572ec.png)      |
|   ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)   |           ![图片不存在](media/67aad2ab2cfe74285da6d91e53385ff4.png)           |
|   ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)   |         ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png)         |

![图片不存在](media/58b75ba1ba6bfa524479ef35a58fcf13.png)

**Conceive:**

1. **Initialization**

   Initialize serial port.

   Create a float variable *voltage* to store the input voltage of the ultraviolet sensor. Assign an initial value of 0 to it.

   Create an integer variable *uv* to store the detected UV index. Assign an initial value of 0 to it.

   ![图片不存在](media/caf13bc617a90f04f6bdc7543c2ed2a8.png)

   ![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

2. **Main Code**

   Loop: print the analog value read by the sensor and the voltage converted from the analog value. The results will be refreshed every 0.1s.

   ![图片不存在](media/e02b91b9071710f66ddd7fa61af3ca89.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![图片不存在](media/35c19374be43897aabd74153f6f4f6bf.png)

   Connect the UV sensor to pin A7, read the analog value of pin A7 and convert it into voltage(V).

   ![图片不存在](media/916a5afdad113ee33b1b024e888dfc5a.png)

   The voltage unit in the Comparison Table is millivolt(mV), so we convert the analog value read by the sensor into voltage in mV. We only need to multiply the value by 1000.

   ![图片不存在](media/71734f6b3606fd8aa15a841e13d0845d.png)

   Assign the converted value to variable *voltage*.

   ② Drag blocks and build as follows:

   ![图片不存在](media/d34d6db98cc3b5afd149d3d9420399f6.png)

   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)

   ![图片不存在](media/67aad2ab2cfe74285da6d91e53385ff4.png)

   If the condition is True, execute the blocks in "if".

   If the condition is False, skip this block.

   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)

   If the voltage is lower than 50mV, variable uv = 0.

   ③ Drag blocks and build as follows:

   ![图片不存在](media/f9b7c8caafb4ee624e565a79ccc0d8ba.png)

   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)

   ![图片不存在](media/19475c6dc699433b285feba386d1cd74.png) determines whether the left value is greater than the right value. If yes, the condition will be output true.

   ![图片不存在](media/acc07e3e4671abf870f3db5769414e09.png): Only when the two conditions are both satisfied, it outputs True.

   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)

   When the voltage is greater than 50 but lower than 227, variable uv = 1.

   ④ Duplicate the block.
   
   ![图片不存在](media/aca77da04320e34441f5696bc255f496.png)
   
   As follows:
   
   ![图片不存在](media/9bf94c6108f071bde4031eb3c503f9b3.png)
   
   Duplicate for 10 times and set the condition according to the Comparison Table:
   
   If voltage < 50 is True, uv = 0.
   
   If voltage > 50 and voltage < 227, uv = 1.
   
   If voltage > 227 and voltage < 318, uv = 2.
   
   ... ...
   
   If voltage > 976 and voltage < 1079, uv = 10.
   
   If voltage > 1079, uv = 11.
   
   ![图片不存在](media/70f05610e4c976b6bfe55a8a38827fe0.png)
   
   We adopt **if** block to determine the range of the UV index.
   
   ⑤ Put into **forever**, as follows:
   
   ![图片不存在](media/a9677876832aafb58fcd16baf4d2189c.png)
   
   Serial monitor prints the voltage value and UV index and refreshes the results every 0.1s.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![图片不存在](media/81687183903f3a617cf2f7088b089c33.png) and set Buadrate to 9600.

![图片不存在](media/6d861659d1bb976ce0da011cb5a31997.png)

After uploading the code, the monitor prints the UV index and the voltage value (mV) converted from analog values of the sensor.

![图片不存在](media/ee2fa452c6b4cc7b43ab0828fffdc8f4.png)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

3.9 Traffic Light Module

![图片不存在](media/0f796489e3fccd806ac608826e78772c.png)

![图片不存在](media/7198611019434fe1aa7380892f0d2835.png)

A traffic light acts as a signal that commands the traffic operation, which is generally composed of red, green and yellow light. Red indicates traffic-prohibited, green means traffic-permitted, and yellow is a warning signal.

This traffic light module is also composed of red LED, yellow and green LED, whose working principle is consistent with that of white LED module.

![图片不存在](media/574fafd11b0076d3a77d6b35961bec45.png)

Parameters

![图片不存在](media/bb22aeac8f0bbe54abccb1cb3e9a155a.png)

Operating voltage: DC 3.3 ~ 5V 

Operating current: 40 mA

Maximum power: 0.2 W

Operating temperature: -10°C ~ +50°C

Dimensions: 48 x 24 x 18 mm (without housing)

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![图片不存在](media/ff61b588417e98ef8df9e4d9834f8c52.png)

Principle

![图片不存在](media/dda544dbaa39b4e95f3be6d8b44aa584.png)

The port of this module is in white, so we need to connect it to the white ports on the board.

![图片不存在](media/352abf053f3755386e8667f1ec35c7dc.png)

In this experiment, we connect the module to port 9. According to the order of the pins, the red LED is connected to pin D9, yellow to pin D10, and green to D11.

When the mainboard inputs high(1) to the module, the connected LED will light up. If it is low(0), the related LED will go off.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/3280168872bdb3cf52a6e38f657a47e1.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **3.9Traffic light module.sb3** file.

![图片不存在](media/1dd9890e4dcb024be0122fb0b43467ee.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Code Blocks**

|            Blocks             |          Code block           |
| :---------------------------: | :---------------------------: |
|  ![图片不存在](media/b235f1924c2c2c6201df43967b104116.png)  |   ![图片不存在](media/7b373bcabc1aed5fc0b05092679a22fa.png)   |
|       ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)       | ![图片不存在](media/fe7119610b2cdfe715aaaba76dbf0757.png) |
|       ![图片不存在](media/fda5fff43c1d402284af13ede3a236f4.png)       |  ![图片不存在](media/5530574a048b6ebc200f7c7d8d974850.png)  |
| ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png) | ![图片不存在](media/27ff2f64a99f85b0f74de875ad5572ec.png) |
| ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png) |    ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png)    |
| ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png) |  ![图片不存在](media/288d63cf54cb7a3c2f31b31d27a2e5d2.png)  |

![图片不存在](media/58b75ba1ba6bfa524479ef35a58fcf13.png)

**Conceive:**

1. **Initialization**

   Set pins and modes.

   ![图片不存在](media/e2053838d5d79e1199779967a6628bfe.png)


![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

2. **Main Code**

   Loop: red LED lights up for 5s; yellow LED blinks for 3 times; green LED lights up for 5s.

   ![图片不存在](media/59f6dcf97c1f282f7d998455a614ef3c.png)

   <br>

   **Build blocks:**

   ① Drag blocks and build as follows:

   ![图片不存在](media/939599c6ef47112b36475d24d7dea061.png)

   Set pin D9 to output high for 5s and then output low: red LED lights up for 5s and goes off.

   ② Drag blocks and build as follows:

   ![图片不存在](media/89b4bd79289ce3d2e9851bbc3633a1c9.png)

   ![图片不存在](media/35ed2fcd5aea903247f69dc65eeeafdc.png)

   ![图片不存在](media/288d63cf54cb7a3c2f31b31d27a2e5d2.png) : codes in this block will run repeatedly, and the times can be set.

   ![图片不存在](media/44ec79a7b20118c7414b12461405431d.png)

   ![图片不存在](media/f2e8071d20a0b3c917f95b1e1b28439b.png)

   The yellow LED turns on for 0.5s and off for 0.5s (blinks for 1s).

   ![图片不存在](media/233b8d9b106ce713d52438f9dfcffda5.png)

   Set the times to 3, so the yellow LED blinks for 3 times.

   ③ Drag blocks and build as follows:

   ![图片不存在](media/ec0373a5a7e59004d99c0de162d7fb4a.png)

   The green LED lights up for 5s and goes off.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, repeat these actions: the red LED lights up for 5s, yellow one blinks for 3 times and green LED lights up for 5s. 

![图片不存在](media/b46d007e9c767f48d4e52e1f360e9b4d.gif)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

3.10 LPS331APTR Air Pressure Sensor

![图片不存在](media/0f796489e3fccd806ac608826e78772c.png)

![图片不存在](media/9792eb8b58f683d734af81a3d6a4133f.png)

Air pressure effects human health physiologically and psychologically.

Low pressure, on the one hand, influences the supply of oxygen. When human body lacks of oxygen, especially the brain, symptoms such as dizziness, headache, nausea, vomiting and weakness may be developed. On the other hand, impairments may also located in the nervous system. Even lung edema and coma may occur, which is commonly known as the "mountain reaction".

High pressure is also having a deleterious effect. It may lead to tinnitus, dizziness, and even the rupture of the eardrum; Decompression sickness can occur if decompression is not done properly after working in a high pressure environment.

Beyond that, air pressure will also change people's psychological moods, causing depressed emotions.



![图片不存在](media/574fafd11b0076d3a77d6b35961bec45.png)

Parameters

![图片不存在](media/bb22aeac8f0bbe54abccb1cb3e9a155a.png)

Operating voltage: DC 3.3 ~ 5V

Operating current: 30 uA

Maximum power: 0.000015 W

Working pressure range: 260 ~ 1260 mbar

Operating temperature: -10°C ~ +50°C

Dimensions: 48 x 24 x 18 mm (without housing)

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![图片不存在](media/ff61b588417e98ef8df9e4d9834f8c52.png)

Principle

![图片不存在](media/dda544dbaa39b4e95f3be6d8b44aa584.png)

LPS331APTR module is with green housing, which is an I2C communication sensor, so we should connect to ports with green on the board.

In this experiment, we connect it to port 5.

![图片不存在](media/4e49ab07b516927b9102f47ec0f3b10e.png)

Before using, we need to import LPS331AP library.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/ffce852695055b06e1f3f1c64027e7f7.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **3.10Air pressure detection.sb3** file.

![图片不存在](media/92a480686d517d0cfb21039c43bda764.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Code Blocks**

|             Blocks              |           Code block            |
| :-----------------------------: | :-----------------------------: |
|   ![图片不存在](media/b235f1924c2c2c6201df43967b104116.png)   |    ![图片不存在](media/7b373bcabc1aed5fc0b05092679a22fa.png)    |
| ![图片不存在](media/860fd6e007ff8448fe077b27662b81e6.png) | ![图片不存在](media/a111d37bb36684ba25d8bed462ba9aa1.png) |
|  ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)  |  ![图片不存在](media/27ff2f64a99f85b0f74de875ad5572ec.png)  |
|  ![图片不存在](media/2d9bb68a76d6f85e82282e3b4833b446.png)  |     ![图片不存在](media/a26b03c713df3254d6a843b1aa8f0d88.png)     |

![图片不存在](media/58b75ba1ba6bfa524479ef35a58fcf13.png)

**Conceive:**

Add library first. Click ![图片不存在](media/62c05ffc94b8065d1e8be8dbf5956696.png) to load **lps331ap** .

![图片不存在](media/e520cf28c9668f9860ea54e0baab2895.png)

1. **Initialization**

   Initialize the serial port.

   ![图片不存在](media/6c40cd60cf76d40a75685a0f05acbaac.png)


![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

2. **Main Code**

   Loop: print the air pressure value and temperature value read by the LPS331APTR sensor. The results will be refreshed every 0.1s.

   ![图片不存在](media/7a35fe55ad511820080f98757b9e480b.png)


![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

<span style="color: rgb(2550, 10, 50);">Set baud rate before uploading code to avoid garbled words.</span>

Click ![图片不存在](media/81687183903f3a617cf2f7088b089c33.png) and set Buadrate to 9600.

![图片不存在](media/6d861659d1bb976ce0da011cb5a31997.png)

After uploading the code, the monitor outputs the pressure and temperature value and refreshes them every 0.1s.

![图片不存在](media/bd113ec21ee35887db54d108789a4597.png)

Touch the sensing area with your finger, and you will see the temperature value rises.

![图片不存在](media/372d0e57149d16fdf4a529113d9b8246.png)

![图片不存在](media/e1bd75bbc77c65e72e1731760b661ca1.png)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

## 4. Comprehensive Experiments

4.1 Rain Detection

This station monitors weather conditions in real time.

In this experiment, we combine a steam sensor and a passive buzzer to achieve a rain detection function for this mini meteorological station. When the steam sensor detects rain, the buzzer alarms. 

Flow

![图片不存在](media/68739b9eba3e04a88586eec60d7fc9ca.png)

Assembly

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Required Parts**

![图片不存在](media/668dd2767382d9d52b8c4c189acc16c7.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 1**

![图片不存在](media/72ee1b98f8676fbd77f8bfd8b44f18a9.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 2**

![图片不存在](media/499530e704634795298458202095ad5c.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 3**

![图片不存在](media/39e658e4d34fdfe5103fd8ea46d2b5db.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 4**

![图片不存在](media/f2223f22e15f0f1201e2ced9d0c80a65.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 5**

![图片不存在](media/a612f004ad2dcb2390cd349537a32329.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 6**

![图片不存在](media/d0c551fe609f044fbfd06794f3ceebec.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 7**

![图片不存在](media/e3c488608724e22735acc9fac9f3c5b9.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 8**

![图片不存在](media/dabd92658af8140a063ee2b33197ee03.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Completed**

![图片不存在](media/0179974542dccfc8ff6b8be2f0669523.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

Wiring Diagram

![图片不存在](media/0cae0ae6a73f064908fca4ac789529da.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **4.1Rain detection.sb3** file.

![图片不存在](media/23f68400a142f672a168c6e0ab7aa58f.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**	

Set a threshold of voltage to determine the water volume. When there is too much water, the voltage exceeds the threshold, rain is detected, and the buzzer alarms. The buzzer will stop alarming when the voltage is lower than the threshold.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization. Set the pins of the steam sensor and the passive buzzer, set the voltage value of a single scale, and set the frequency of the passive buzzer.

   ![图片不存在](media/62d529b93b0e6b1e2f4ca8bbccfe6ac3.png)

2. Loop:

   Print the analog value and voltage of the steam sensor.

   Determine whether the voltage exceeds 1 (<span style="color: rgb(10, 10, 200);">Herein, we set 1 as the threshold, which is adjustable according to needs</span>).

   - voltage > 1: buzzer alarms.
   - voltage ≤ 1: buzzer does not emit sounds.

   ![图片不存在](media/1ea85f8e42e1418055bbc747a2c85db1.png)

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, the steam sensor will detects the ambient water volume and converts it to a voltage output. When the voltage is greater than 1, the buzzer alarms. If not, the buzzer will not emit sounds.

<span style="color: rgb(2550, 10, 50);">**ATTENTION: Be careful when using water, please do not to drip to any other place outside the detection area to aviod a short circuit.**</span>

![图片不存在](media/71fed73fa89c2d7b7b4e3d936c8a9206.gif)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

4.2 Fire Alarm

The fire alarm system of the station can effectively prevent and deal with forest fires.

In this experiment, we build a fire alarm with a flame sensor and a passive buzzer. When flame is detected, the buzzer will emit sounds for alarming. 

Flow

![图片不存在](media/2860a693e50904d0c22e6eade5a8c440.png)

Assembly

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Required Parts**

![图片不存在](media/52cf38f0c8ebe681d5944ff75d8cb6c8.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 1**

![图片不存在](media/6de6d32c05cd762207f811692f9645fa.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 2**

![图片不存在](media/23b2a3a5a34c9ebcedd2cc7feff4a349.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 3**

![图片不存在](media/d56dcc94ae490773d04d66794e1d8633.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 4**

![图片不存在](media/ccea7ef564d9db2a9da94f73633675c9.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 5**

![图片不存在](media/d5119b491d04aa12dfe213f60f1379f4.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 6**

![图片不存在](media/f6255134f649fbe817598fb324f305b4.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 7**

![图片不存在](media/ddf133353beaadaa52c630efe1a1cb3b.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 8**

![图片不存在](media/06698f4cfc017346049a1ca6cf920357.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Completed**

![图片不存在](media/414176f6673cde2f461c2d89b1bca116.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

Wiring Diagram

![图片不存在](media/ef6e599365d4921281d0d17ad69e4085.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **4.2Fire alarm.sb3** file.

![图片不存在](media/517d976244c30bc10b7499046156de69.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**

Set a threshold of voltage to determine whether there is flame. When the sensor detects flame, the voltage is lower than the threshold, and the buzzer alarms. The buzzer will stop alarming when the voltage exceeds the threshold (the sensor detects no flame).

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization. Set the pins of the flame sensor and the passive buzzer, set the voltage value of a single scale, and set the frequency of the passive buzzer.

   ![图片不存在](media/5ec9135e4041d749920c4aeaf3154358.png)

2. Loop.

   Print the analog value and voltage of the flame sensor.

   Determine whether the voltage is lower than 4 (<span style="color: rgb(10, 10, 200);">Herein, we set 4 as the threshold, which is adjustable according to needs</span>).

   - voltage < 4: buzzer alarms.
   - voltage ≥ 4: buzzer does not emit sounds.
   
   ![图片不存在](media/69dcae2c5da53b2836962655698d3a3d.png)

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

Upload the code. When the flame sensor detects flame, the voltage will lower than 4, and the buzzer will alarm. If not, the buzzer will not emit sounds.

![图片不存在](media/07ede3488c0f57d2e61ed58e76416f98.gif)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

4.3 Magnetic Field Detection

After the lightning strike, a certain amount of electricity will generated in the surrounding, and a strong magnetic field will be produced in an instant. 

This magnetic field interferes with the connection of the relevant equipment of the station, thus disabling the automatic devices. Therefore, it is necessary to detect the magnetic field at all times and alarm immediately when the magnetic field is detected.

In this experiment, we utilize a Hall sensor and a white LED module to detect magnetic field. When the Hall sensor detects a magnetic field, the white LED lights up.

Flow

![图片不存在](media/bd8bc7dc51edb15ab56e90e1b3a3b260.png)

Assembly

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Required Parts**

![图片不存在](media/a0757e59a99ce5cdc8c4bd63366b3cd3.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 1**

![图片不存在](media/f86308ab94f949ecf77e06cdbc23c15b.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 2**

![图片不存在](media/81e10d4791b4b6aec20238f37c493aae.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 3**

![图片不存在](media/ba12d32f1e2ee9a1524e3c8c49dd2bd8.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 4**

![图片不存在](media/cc241419ca42e9ba125b54b10776274a.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 5**

![图片不存在](media/0cd2f7377d0deeb1d76d345ff2480ec9.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 6**

![图片不存在](media/adc1bbfb57eb472b89bd6c02ac42cc15.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 7**

![图片不存在](media/d8277bcc6b09ed294039ceb9cd9770ed.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Completed**

![图片不存在](media/3d5f8e842bda98fa7354987fc6b7b4b7.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

Wiring Diagram

![图片不存在](media/3e9c7933764bc99d741373ece4091468.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **4.3Magnetic field detection.sb3** file.

![图片不存在](media/650f4c7b984cd30c2199a5326facef1a.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**

When the Hall sensor detects a magnetic field, a low power(0) will be output, and the white LED lights up. If there is no magnetic field, high(1) will be output, and the LED goes off.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization. Set the pins of the Hall sensor and the white LED module.

   ![图片不存在](media/6d8be5357ac54088296cb057092a3e61.png)

2. Loop.

   Print the digital value of the power level of the Hall sensor.

   Determine whether the value equals 0 (0 means a magnetic field is detected). 

   - value = 0: the white LED lights up.
   - value ≠ 0: the white LED goes off.

   ![图片不存在](media/58609f3c666653c2234a5d476377ba4c.png)


![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, the Hall sensor starts to detect magnetic field.

If the sensor detects a magnetic field, the white LED will turn on. If not, the LED will go off.

![图片不存在](media/97377a5dee3ef21e6b9d98c7a1df470a.gif)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

4.4 Thunder Detection

Thunder is the atmospheric sound produced by lightning. When thunder is detected, it sends an alert that rain may be coming.

In this experiment, we integrate a sound sensor and a white LED module to construct a thunder detector. When the thunder volume exceeds a set threshold, the white LED will lights up.

Flow

![图片不存在](media/926d61ac26eb6307c74266bc20b53f4e.png)

Assembly

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Required Parts**

![图片不存在](media/0da61e437d1f482051c6d7998a3f2c4e.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 1**

![图片不存在](media/fe786304d8f096dd119a6ba6901bb21a.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 2**

![图片不存在](media/db20f1b299a2b67a8a35f60816e71e43.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 3**

![图片不存在](media/09958a8f58a27dc300bd59c29678f7b8.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 4**

![图片不存在](media/e9531dd1d9bb6b3f378bdf1fd45f5410.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 5**

![图片不存在](media/9ca55af68b595d65870a37f3ff56d845.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 6**

![图片不存在](media/1c779230910422b86a80f8279d9395e8.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 7**

![图片不存在](media/fc6adb99c821d9e3378a6c46b50e2543.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Completed**

![图片不存在](media/924d8ade589d186ae8637f11c2fc15b9.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

Wiring Diagram

![图片不存在](media/5f4f2e0e93f00a2b3138da097cbf4556.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **4.4Sound detection.sb3** file.

![图片不存在](media/e950e37494e0a57ba85f2f48e7f1d64e.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**

Set a threshold of analog value to determine the thunder volume. When thunder is detected, the analog value exceeds the threshold, and the white LED lights up as an alarm. The LED will go off when the value is lower than the threshold.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization. Set the pins of the sound sensor and the white LED module.

   ![图片不存在](media/e6ed74f35dc9ddd944821275ab0f135c.png)

2. Loop.

   Print the analog value of sound volume detected by the sound sensor.

   Determine whether the analog value is greater than 100 (<span style="color: rgb(10, 10, 200);">Herein, we set 100 as the standard threshold of thunder volume, which is adjustable according to needs</span>).

   - analog value > 100, the white LED lights up.
   - analog value ≤ 100, the white LED goes off.
   
   ![图片不存在](media/a340e438c41476836e4abea0a82c3b25.png)

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, the sound sensor detects whether there is a thunder. When the analog value of the sound exceeds 100, a thunder is detected and the white LED will light up.

Here we stimulate thunder by playing music. When the value is greater than 100, LED lights up.

![图片不存在](media/0adbf9cc90f58d97990ea9b3cb5fe64a.gif)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

4.5 Temperature Detection

It is necessary to monitor the atmospheric temperature in the natural environment in real time. If the temperature is too high, disasters such as fire may occur. When the normal temperature is detected, the green LED lights up; the yellow LED is a reminder for raising temperature; if red LED is on, be very careful because it indicates a high temperature!

In this experiment, the XHT11 temperature and humidity sensor and the traffic light module to measure temperature range. Three colors of LED indicate three ranges of ambient temperature. 

Flow

![图片不存在](media/92f231d00b82599a16cd042f2c404b32.png)

Assembly

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Required Parts**

![图片不存在](media/260e654ff76eef3862a782225fe43eb9.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 1**

![图片不存在](media/b27745a041067c2705eb90555b3671f4.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 2**

![图片不存在](media/dd1ff7fcce38303faeabbfef77ad8209.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 3**

![图片不存在](media/6968f988bf1b29a065a46eff399abd5b.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 4**

![图片不存在](media/fd17d839912b892766339eba04b6ca42.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 5**

![图片不存在](media/97edee6113a8e371c4ecbb65a7f5cfb8.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 6**

![图片不存在](media/38b47b800997b2a1d1e13ae7f16aeb6b.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Completed**

![图片不存在](media/63bf01c075cc0d4d854502e67ce157a4.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

Wiring Diagram

![图片不存在](media/188a3e573095d520595f0cdf67d7c5a4.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **4.5Temperature detection.sb3** file.

![图片不存在](media/509d4e1dfd60332954ed37c837b8b400.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**

Set three thresholds to separate the temperature range: 24, 29, 35, which are adjustable according to needs.

- preference temperature: 24°C ~ 29°C
- warning temperature: 29°C ~ 35°C
- high temperature: over 35°C

Corresponding LED will light up when the ambient temperature is within the related ranges.

- Within preference temperature range: the green LED lights up
- Within warning temperature range: the yellow LED lights up.
- Within high temperature range: the red LED lights up.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization. Set the pins of XHT11 temperature and humidity sensor and the traffic light module.

   ![图片不存在](media/e5f5b544d581a473beb5069c8c525599.png)

2. Loop.

   XHT11 sensor reads and outputs the temperature values.

   Determine which section the temperature value is in, so then light up corresponding LED.

   - 24°C ≤ temperature < 29°C: the green LED lights up and other LEDs are off.
   - 29°C ≤ temperature < 35°C: the yellow LED lights up and other LEDs are off.
   - temperature > 35°C: the red LED lights up and other LEDs are off.
   
   ![图片不存在](media/cd3d83e53e3170aaff69a63d83e670c4.png)

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, the XHT11 sensor detects the ambient temperature value.

When the value is in the preference temperature range, the green LED lights up;

When the value is within the warning temperature range, the yellow LED turns on;

When the value exceeds the high temperature threshold, the red LED lights up.

![图片不存在](media/525e9ee10b46ccf3dfd4a32cbfc24c53.gif)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

4.6 Ultraviolet Detection

In daily life, when the UV index is greater than 3, you'd better do sunscreen measures when going out. This station will calculate the UV index in real time to make timely reminders.

In this experiment, we detect the UV index with an ultraviolet sensor and a traffic light module. When the detected UV index is higher than a set threshold, the red LED will light up.

Flow

![图片不存在](media/963f0500563a5475c7c7cca18957809e.png)

Assembly

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Required Parts**

![图片不存在](media/9d66023baa1dcfb5162c864c3c96d7c4.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 1**

![图片不存在](media/5b833078a67b5a846d314acfec93b963.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 2**

![图片不存在](media/56d5597e4413006b525cdfb36af13326.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 3**

![图片不存在](media/f21fc29eb3436bbf49ac9a2d0488fcf1.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 4**

![图片不存在](media/ab78dd16a2499e31108b27c92d9b565e.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 5**

![图片不存在](media/269a148802b930ce2e89aa0d61bc7d31.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 6**

![图片不存在](media/749965e3af108da858a8a75d323b077d.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 7**

![图片不存在](media/5e6185623f7b33bed5ae1926e1fcea11.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Completed**

![图片不存在](media/e225b921268892cd261ff256d1bd55be.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

Wiring Diagram

![图片不存在](media/e423e5606aecdf22cb4668f33e17b880.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **4.6Ultraviolet detection.sb3** file.

![图片不存在](media/6c4b86c89068a19f66a47d290058c427.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**

When the UV index is within 0 ~ 2, the ultraviolet light is the weakest, and it does not have much effect on the human body. When the index increases to 3 ~ 4, the ultraviolet light is weak, but remember to wear sunscreen when going out. 

Herein, we set the threshold of the UV index to 3. If the value exceeds 3, the red LED will light up to remind you to wear sunscreen. If the value does not reach 3, the LED will go off.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization.

   ![图片不存在](media/c21d42b28524046a796cf28ca414b856.png)

2. Loop:

   if elif statement to determine the range of UV index, and output the value.

   Determine whether the UV index exceeds 3.

   - UV index > 3: the red LED lights up as a reminder.
   - UV index ≤ 3: the red LED goes off.
   
   ![图片不存在](media/05c061466949b2b7d33786b457d0d413.png)

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, when the UV index is greater than 3, the red LED will light up to remind you to take sun protection measures when going out.

![图片不存在](media/bc1b7fb876c256f6d4f7127f91e93611.gif)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---
4.7 Air Pressure Detection

The station monitors air pressure in real time. When the air pressure is in normal range, the green LED lights up; When it is in the low range, the yellow LED turns on; When it is high, the red LED is on.

In this experiment, we use an LPS331APTR air pressure sensor and a traffic light module to reveal the air pressure. LED will light up in corresponding colors when the pressure value is in the related set range.

Flow

![图片不存在](media/f508427f4d260c90191cf7162370eae3.png)

Assembly

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Required Parts**

![图片不存在](media/ef4b52a495a1f34c52f16a1db9f7427a.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 1**

![图片不存在](media/9671348396f252ed46af2ed29b048250.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 2**

![图片不存在](media/f2269238892afb6150323e1decfe759e.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 3**

![图片不存在](media/22de8e93ff1e063b3c089fa7f694609d.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 4**

![图片不存在](media/e70ca9d932469fc42f2aaa0e6ac0361d.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 5**

![图片不存在](media/84ac495795ecf8b8c7a3312665f16626.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 6**

![图片不存在](media/2ca6903e9b9f010891777a7f565eb907.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 7**

![图片不存在](media/6929988fb26d0a1132ff4718adf880e3.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 8**

![图片不存在](media/6c4764786c83678c16a8a112e049a515.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 9**

![图片不存在](media/10efe116a687a3a59804cab69f7f3715.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Completed**

![图片不存在](media/d078547f4346561b2924f1b5b1cd803a.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

Wiring Diagram

![图片不存在](media/85d820428928fb1e55d39658adfdeaa8.png)

Test Code

Open KidsBlock and connect the board to your computer. Click **File --> Load from your computer**.

![图片不存在](media/769cddbf76a3c1810a85f38a006ca505.png)

Choose D:\Code\1.Code_kidsuno to open **4.7Air pressure detection.sb3** file.

![图片不存在](media/f707debdbdde0a3512fa5a3a82b77eb4.png)

Click ![图片不存在](media/a008c7eb767f0f7aecbaf941f4b4b18a.png)to connect to port and then  ![图片不存在](media/251c1ea677e15869efc8ec5862a2204b.png).

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

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

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization. set the pins of LPS331APTR air pressure sensor and the traffic light module.

   ![图片不存在](media/62b98c28e36df32b106312d0bd761dca.png)

2. Loop.

   LPS331APTR sensor reads the air pressure value and outputs it.

   Determine which range of the pressure value is in, in order to turn of related LED.

   - air pressure > 1050hPa: the red LED lights up and other two LEDs goes off.
   - air pressure < 950hPa: the yellow LED lights up and other two LEDs goes off.
   - 950hPa < air pressure < 1050hPa: the green LED lights up and other two LEDs goes off.

   ![图片不存在](media/c7ec6c266c8b25fcbc2dab24ab772bb6.png)

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, the LPS331APTR sensor measures the air pressure.

When the air pressure is in normal range, the green LED lights up;

When the air pressure is in the low range, the yellow LED lights up;

When the air pressure is in the high range, the res LED turns on.

![图片不存在](media/8ed5aa7ca790e59dcc52115d19338975.gif)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

