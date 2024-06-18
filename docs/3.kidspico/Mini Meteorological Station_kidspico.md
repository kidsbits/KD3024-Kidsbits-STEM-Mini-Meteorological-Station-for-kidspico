# Mini Meteorological Station for kidspico



## 1. Code and Firmware

[DOWNLOAD](../Code.zip)

Download and unzip these files. Here all codes are in folder **3.Code_kidspico** and firmware is at  **3.Firmware_kidspico**.

For convenience, <span style="color: rgb(2550, 10, 50);">we move the codes into: **D:\Code\3.Code_kidspico**.</span> You can also choose to move it into any disks at will. 

---



## 2. Development Environment Configuration

2.1 Thonny Download

Windows

**We demonstrate on Windows 10.**

Download: [Thonny Official](https://thonny.org)

Click **Windows** to choose one version to download.

![图片不存在](media/1da314fdb9460667dbfd3a4697d7d815.png)

![图片不存在](media/f71c729288441acf01675ae9cad173fa.png)

MAC

Similar to Windows.

![图片不存在](media/f517b5c778eb9e172ca7372f9e4c5206.png)

![图片不存在](media/ed892528a3b824fea39e6ac7c55b507e.png)

2.2 Thonny Installation

Two methods:

- Install Thonny+Python package

	Recommended for beginners: When you install, the Python environment and Thonny will be packaged so both installed. There are also two ways to install the package:

	- Installer

		![图片不存在](media/25dd356cfd9dfd55ecbdb0b92c5c9b46.png)

	- Portable variant

		![图片不存在](media/678a9e354e95415065e0778a31f528a1.png)

- Install Thonny only

  Recommended for developers: When the user already has a python environment, `pip install thonny` comes in handy to install Thonny separately.

  ![图片不存在](media/94f0fd8a4fa3a9175c15b6888f4544f2.png)

Please just install according to your needs.

Installer

Here we demonstrate how to install `Installer with 64-bit Python 3.10` on <span style="background:#ff0;color:#000">64bit Windows 10</span>.

(1）After downloading, click![图片不存在](media/338a61d9cff83564996f495080f416ac.png) . And you will see **Select Setup Install Mode**, choose **Install for me only**.

![图片不存在](media/88a462f0aaa7ad0f4942f99d422d8334.png)

(2） **Next** 

![图片不存在](media/c1460a4ddcd3cfafd15715dd853cce8e.png)

(3）Tick **I accept the agreement** and **Next**.

![图片不存在](media/fbdc3f05f83a9307844ec71b33d073c0.png)

(4）The default path is Disk C, or you can click **Browse...** to modify the path. After that, click **Next**.

![图片不存在](media/927100ee3afa1898f8838ce20b320778.png)

(5）Choose a path to create the program's shortcuts, and click **Next**.

![图片不存在](media/8f07d7269aa8712708ced638a2f11520.png)

(6）Tick **Create desktop icon** and click **Next**.

![图片不存在](media/b174adb8f5e2ec634231f56c218bca66.png)

(7）Inatall 

![图片不存在](media/1ec304475b437048c292b2fc681d035b.png)

(8）“**Finish**”

![图片不存在](media/b76a5b738925fee9067972e32c623904.png)

(9）Open Thonny and choose your language.

![图片不存在](media/ead3ab9ec7ccfc8b0868be0b49b909b4.png)

(10）Main interface:

![图片不存在](media/a306e5906d179d1ff414e7b2719ecc50.png)

Portable Variant

Here we demonstrate how to install `Portable variant with 64-bit Python 3.10` on <span style="background:#ff0;color:#000">64bit Windows 10</span>.

(1）After downloading and being unzipped, click ![图片不存在](media/0217a936fef31e9b5cd9746e14bdbc3e.png) to choose your language.

![图片不存在](media/ead3ab9ec7ccfc8b0868be0b49b909b4.png)

(2）Main interface:

![图片不存在](media/a306e5906d179d1ff414e7b2719ecc50.png)

(3）For convenience, please send ![图片不存在](media/989d968b70ef76f419148e56237f4b73.png) to Desktop(create shortcut).

![图片不存在](media/24b758a58e44e004e2268a1e4d9e6343.png)

Shortcut: ![图片不存在](media/c09110399ccfb7dd7ec25a6837aade3e.png)

---

2.3 Firmware

Press and hold the BOOT button on the kidspico mainboard, connect it to PC via USB cable and then release the BOOT button. 

A removable hard disk will show up.

Open folder **3.Firmware_kidspico**, find and copy the firmware ![图片不存在](media/43b4b7f9196fe802d033df8122d36de0.png) into this disk.

![图片不存在](media/0a41cb38660c2588db2e2177c5fac490.png)

After that, open Thonny to connect to port (COM number varies from devices). 

![图片不存在](media/64e1bb12fbdbbab05685ef622b0dc7db.png)

---

2.4 Thonny

Interface

Click **View** and tick **Files** to open the file path management.

![图片不存在](media/96b321dd12559ae0431ab769e4881d3e.png)

![图片不存在](media/66ec7c77b9e71d0153a0a768bbda8ae1.png)

Toolbar

![图片不存在](media/def0d20d9c2937b70b683e9c628c9bfe.png)

|          ICON           |            FUNCTION            |
| :---------------------: | :----------------------------: |
| ![图片不存在](media/1ca46b3024b5eb56a64f9e51fb5b6bda.png) |          New (Ctrl+N)          |
| ![图片不存在](media/09eb106daa19a6839389b861c0189eb8.png) |        Open... (Ctrl+O)        |
| ![图片不存在](media/6165658942fac7b66d707bf8c138e261.png) |         Save (Ctrl+S)          |
| ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png) |    Run current script (F5)     |
| ![图片不存在](media/5b1e3fe0bca1c55b4b836513ca80b250.png) |      Debug current script      |
| ![图片不存在](media/1db201db2164fd4add0190cc9960e5fc.png) |         Step over (F6)         |
| ![图片不存在](media/b4e2114fed530be1ebcccf33204d9b44.png) |         Step into (F7)         |
| ![图片不存在](media/b3b8f253dd39dc4996401f94b70f953c.png) |            Step out            |
| ![图片不存在](media/772d4d8c7b2426ca1c7b9843947b8ae4.png) |          Resume (F8)           |
| ![图片不存在](media/dc7b8f052ee9198b54f12392d91d4171.png) | Stop/Restart backend (Ctrl+F2) |

---

2.5 Test

<span style="color: rgb(2550, 10, 50);">Please download and unzip code files and save them in a path as your need. For instance, **D:\Code\3.Code_kidspico**.</span>

In Files, click **This computer**.

![图片不存在](media/783512ccf54871000cf504915a1e07d6.png)

Enter **Disk D** and open folder **Code**, find **3.Code_kidspico** and you will see all codes.

![图片不存在](media/c74fca08585092681a160922b86aaa24.png) ![图片不存在](media/00672cbe77dde615a6c221deb183baee.png) ![图片不存在](media/a5bd23f7d9c5a8bb58956ab2c53bd692.png)

Connect to kidspico and choose COM port. 

![图片不存在](media/19e971320f9aea85ab005f755b97288f.png)

Test Shell Command

Input the following code in Shell.	

```python
print('hello world')
```

![图片不存在](media/fb2d12dcfb12dfa47e06709d8deaffee.png)

Press "Enter" and the Shell prints **hello world**.

![图片不存在](media/e53cb8a3cd7799d413e668daf21e467b.png)

---

Test Online Running

Click to open code **Onboard_LED.py**.

![图片不存在](media/d748a13d2f91d3267b6f52536f329a60.png)

Click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png) to run the code, and the yellow LED on kidspico board will flashes: on for 1s and off for 1s.

![图片不存在](media/fb558cc8643eb22477758eb64da45f46.gif)

---

Test Offline Running

Open **Onboard_LED.py** in Files: File --> Save as... 

Click ![图片不存在](media/1ca46b3024b5eb56a64f9e51fb5b6bda.png) to create a new script, copy and paste Onboard_LED.py in it.

![图片不存在](media/1e7753ff81d1f10725037bd3583ba6f9.png)

Click ![图片不存在](media/6165658942fac7b66d707bf8c138e261.png) to save it to Raspberry Pi Pico.

![图片不存在](media/5442d6b89f57ce083cb5b27428b0bc87.png)

We name it as **main.py**.

![图片不存在](media/c13e40c5484183e9591d9c81b7821603.png)

After saving, the main.py code will automatically execute as long as the kidspico board is powered on. You will see the yellow LED flashes per second. 

![图片不存在](media/75e025ff18a6955748fd47c10c4dfd1c.png)

---

## 3. Modules

<span style="color: rgb(2550, 10, 50);">Please move the codes to a convenient path as your needs, for instance, path: **D:\Code\3.Code_kidspico**.</span>

Kidspico Ports View

During experiments, <span style="color: rgb(2550, 10, 50);">modules can only be connected to ports in the same color.</span>

![图片不存在](media/9a058aa13b94ce84f19de3a2f611a348.png)

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

![图片不存在](media/4010a09457ccb90a934a457c17ece36a.png)

In this experiment, we connect the white LED module to port 1. According to the board ports view, the digital io pin at port 1 is io11.

When we set the pin to high(1), the LED lights up in white; if we set to low(0), it will be off.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/306b5e05a127b7189a3537a988f75ac9.png)

Test Code

Open Thonny and connect to COM port. Open **3.1Light_on.py** in **Files** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Light_on
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import Pin
import time

led = Pin(11, Pin.OUT)  # Set an led object and connect it to pin 11, set pin to output
while True:
    led.on()       # led on
    time.sleep(1)  # delay 1s
    led.off()      # led off
    time.sleep(1)  # delay 1s
```

Explanations

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

1. `from machine import Pin`

   Import Pin from machine to enable its functions.

![图片不存在](media/2fd65b883dd17bd50a77af9b5bdb37c2.png)

  **machine.pin**

```python
machine.Pin(id,mode,pull,value)
```

   - id ：GPIO number, within 0-29. For example, if you enable GPIO11, fill in with 11.

   - mode ：pin mode can be one of the followings:

	​	Pin.IN(0) - set pin to input

	​	Pin.OUT(1) - set pin to (normal)output

	​	Pin.OPEN_DRAIN(2) - set pin to open drain output

   - pull ：specifies whether the pin is connected to a (weak-)pull resistor; it is valid only at input mode, and can be one of the followings:

	​	None - no pull-up/down

	​	Pin.PULL_UP(1) - enable pull-up resistor

	​	Pin.PULL_DOWN(2) - enable pull-down resistor

   - value ：only work at Pin.OUT and Pin.OPEN_DRAIN mode; assign the initial output pin value. Or else, the peripheral state of the pin stays still. 0 is low(off) while 1 is high(on).

   - Pin.on() - set pin to high

   - Pin.off() - set pin to low

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

2. `import time`

   Import **time** type so that its related functions can be adopted.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

3. `led = Pin(11, Pin.OUT)`

	Set LED pin io11 to output mode.

![图片不存在](media/2f5f4d9ef54812ea08960cca8a8806e8.png)

Q ：Why "output"?

A ：The code is written for the mainboard. For the board, pin io11 is outputting power levels (high or low) to the connected module.

![图片不存在](media/bcc144c573b815d3bad3fed954f006c2.png)

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

4. `while True:`

   Statements in this function will execute in a loop.

   Formula of while loop function:

```python
while (condition):
    (statements)
```

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

5. `led.on()` and `led.off()`

   At pin io11 on the mainboard, respectively output high(1) and low(0); i.e., output high(1)/low(0) to LED module to make it on/off.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

6. `time.sleep(1)` 

   Delay 1s.

   ![图片不存在](media/2f5f4d9ef54812ea08960cca8a8806e8.png)

   Q ：Why delay?

   A ：If you output a high level to LED, it will be always on. Yet, we add a delay of 1s, so it lights up for only 1s. Delay time is the ON/OFF time of LED.
   
   ![图片不存在](media/bcc144c573b815d3bad3fed954f006c2.png)

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading code, the LED module will flash with an interval of 1s (on for 1s and off for 1s).

![图片不存在](media/d60aa95d6e9040d62f3c15db68fb6d66.gif)

Click ![图片不存在](media/dc7b8f052ee9198b54f12392d91d4171.png) or Ctrl+C to exit the execution.

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

Dimensions: 32 x 24 x 18 mm（without housing）

Positioning hole: diameter of 4.8mm

Interface: Telephone socket

![图片不存在](media/ff61b588417e98ef8df9e4d9834f8c52.png)

Principle

![图片不存在](media/dda544dbaa39b4e95f3be6d8b44aa584.png)

This Hall sensor is able to distinguish magnetic field north and south. The front of the magnetic induction element (with numbers) senses the South Pole, while its back detects the North Pole.

![图片不存在](media/6aee28639f5ba48880bea0cc37ffd40b.png)

Modules with blue housing are digital ones, so we should connect to digital io pins of the mainboard (ports with blue).

![图片不存在](media/4010a09457ccb90a934a457c17ece36a.png)

In this experiment, we connect the Hall sensor module to port 2. According to the board ports view, the digital io pin at port 2 is io8.

When a magnetic field is detected, Hall sensor outputs low; When no magnetic field is detected, the sensor outputs high.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/eabceb4db79d82216879279daade4382.png)

Test Code

Open **3.2Hall sensor.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Hall sensor
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import Pin
import time

hall = Pin(8, Pin.IN)
while True:
    value = hall.value()
    print(value, end=' ')
    if value == 0:
        print("A magnetic field")
    else:
        print("There is no magnetic field")
    time.sleep(0.1)
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

1. `hall = Pin(8, Pin.IN)`

   Connect Hall sensor to pin io8 and set it to input mode.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

2. `value = hall.value()` 
   
   Assign the power level output by the sensor to  `value`.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

3. `print(value, end=' ')` 
   
   Print value without wrapping, and end with space.
   
   ![图片不存在](media/2fd65b883dd17bd50a77af9b5bdb37c2.png)
   
   `print()`  will wrap to output results **by default**, because there is a **line break** `end ='\n'` which is usually omitted.
   
   In this code, we add `end=''` which will output a space at the end, so the default line break will be canceled. By doing this, the contents will be output without wrapping. 
   
   `end=' '`: add a space at the end rather than a line break.
   
   ![图片不存在](media/2f5f4d9ef54812ea08960cca8a8806e8.png)
   
   Q ：Why Space?
   
   The value will be too close to the contents, which is not convenient for us to check the outputs.
   
   Without space (`end=''`):
   
   ![图片不存在](media/33b6c70105961dd45189bd03d93ab607.png)
   
   With space (`end=' '`):
   
   ![图片不存在](media/9c77df605791e522124ef903afecb9e4.png)
   
   A ：We add a space to separate the value and contents.
   
   ![图片不存在](media/bcc144c573b815d3bad3fed954f006c2.png)
   
   

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

4. ```python
   if value == 0:
       print("A magnetic field")
   else:
       print("There is no magnetic field")
   ```

   **if statement**

   value = 0 (return True): Shell prints *A magnetic field*

   value ≠ 0 (return False): Shell prints *There is no magnetic field*

   ![图片不存在](media/2fd65b883dd17bd50a77af9b5bdb37c2.png)

   The process flow of if statement:

   ![图片不存在](media/cae5fe19879ff100ee40d508a997098d.png)

   Running Principle: pose a condition to determine the trend of next step. If the condition is true, execute the code under this condition. If false, exit the execution.

   In Python, any non-zero/non-empty object is true, and everything else except true and None is false.
   
   - any non-zero/non-empty object is True
   - number 0, empty object and None are False
   - outputs are only True or False.

   Basic composition of an **if statement**:
   
   ```python
   if condition_1:
       statement_block_1
   else:
       statement_block_2
   ```

   If "condition_1" is True, execute "statement_block_1".

   If "condition_1" is False, skip "statement_block_1" to run "statement_block_2".

   Basic composition of an **if elif statement**:
   
   ```python
   if condition_1:
       statement_block_1
   elif condition_2:
       statement_block_2
   else:
       statement_block_3
   ```

   If "condition_1" is True, execute "statement_block_1" .

   If "condition_1" is False, skip "statement_block_1" to determine "condition_2".

   If "condition_2" is True, execute "statement_block_2" .
   
   If "condition_2" is False, skip "statement_block_2" to run "statement_block_3".

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

5. `time.sleep(0.1)`

   Delay 0.1s to stabilize the output, otherwise the Shell will print results at a very fast speed.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, when the **South Pole** of the magnet approaches to the front of the magnetic induction element, the red LED lights up and Shell prints *0  A magnetic field*; 

![图片不存在](media/c0741f51c46a8a5e6f438d87bc5de92b.png)

When the **South Pole** of the magnet approaches to its back or is away from the sensor, the red LED goes off, and Shell prints *1  There is no magnetic field* .

![图片不存在](media/4afb5ba7145d0fdc2462f3e86d6c4928.png)

Put the **North Pole** of the magnet to the back of the element, the red LED lights up and Shell prints *0  A magnetic field*; 

![图片不存在](media/2cfffb7160fc70c2f1243b59c1dc6ccf.png)

Put the **North Pole** of the magnet approach to the sensor or is away from its back, the red LED goes off, and Shell prints *1  There is no magnetic field*.

![图片不存在](media/9d826c2ebf795347d3d574cc08af4b5e.png)

![图片不存在](media/cf8f1b2bc6c97ce11a4e4f5200dcb0b9.gif)

Click ![图片不存在](media/dc7b8f052ee9198b54f12392d91d4171.png)or click Ctrl+C to exit execution.

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

Dimensions: 48 x 24 x 18 mm（without housing）

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

  $ T= \frac {1}{f}$      $ cycle = \frac {1}{frequency}$

  If the frequency is 50Hz, the cycle will be 20ms, i.e., there are 50 PWM cycles in one second.

- **PWM duty cycle**: the ratio of high level time to the whole cycle time.

  - Unit: %(1% ~ 100%)

  
  - Cycle: The time of a pulse signal. The number of cycles in 1s equals the frequency.
  - Pulse width time: high level time.
  
  ![图片不存在](media/89e6481176c78795322869df5feff457.gif)

  <center>The relationship between duty cycle and LED brightness.gif<center>

  The longer the high level time is, the greater the duty cycle will be, and the brighter the LED will be.



**The PWM frequency corresponding to notes**:

![图片不存在](media/bd6f281865cd802b82db6bc86bbe502f.png)

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

Modules with blue housing are digital ones, so we should connect to digital io pins of the mainboard (ports with blue).

![图片不存在](media/4010a09457ccb90a934a457c17ece36a.png)

In this experiment, we connect the passive buzzer to port 3. According to the board ports view, the digital io pin at port 3 is io3.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/dc3c31b99bc5b0055bfc74dbd2ec8b68.png)

Test Code

Open **3.3Passive buzzer.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Passive buzzer
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import Pin, PWM
import time

buzzer = PWM(Pin(3))

'''
-----------------------------
| Pitch names |  Frequency  |
|---------------------------|
|      C      |     523     |
|      D      |     587     |
|      E      |     659     |
|      F      |     698     |
|      G      |     784     |
|      A      |     880     |
|      B      |     988     |
-----------------------------
'''
a = [523,587,659,698,784,880,988]

while True:
    #Tone of duty cycle = 1000
    for i in a:
        buzzer.duty_u16(1000)
        buzzer.freq(i)
        time.sleep(0.2)
    #Tone of duty cycle = 5000
    for i in a:
        buzzer.duty_u16(5000)
        buzzer.freq(i)
        time.sleep(0.2)
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

1. `from machine import Pin, PWM`

   Import PWM function.
   
   ![图片不存在](media/2fd65b883dd17bd50a77af9b5bdb37c2.png)
   
    **machine.PWM**
   
      - `machine.PWM(pin)`: PWM object function, set the specified GPIO to re-initialize and set the mode of PWM output. 
   
        pin: is the GPIO object whose PWM output needs to be set.
   
      - `PWM.freq（value）`: set the PWM output frequency. 
   
        value: PWM output frequency. The value should conform to the PWM frequency calculation formula.
   
      - `PWM.duty_u16（value）`: set duty cycle. Corresponding values will be automatically calculated.
   
        value: Set duty cycle ratio within 0-65536.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

2. `buzzer = PWM(Pin(3))` 

   Connect the passive buzzer to pin io3, output PWM.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

3. `a = [523,587,659,698,784,880,988]`

   Create a list **a** and put elements in [ ], including 523, 587, 659, 698,7 84, 880, 988, which are correspond to frequency of C, D, E, F, G, A, B.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

4. ```python
   #Tone of duty cycle = 1000
   for i in a:
   	buzzer.duty_u16(1000)
       buzzer.freq(i)
       time.sleep(0.2)
   ```

   **for loop**: play tones when the duty cycle is 1000, each tone is played for 0.2 seconds.

   ![图片不存在](media/2fd65b883dd17bd50a77af9b5bdb37c2.png)

   In Python, a for loop is an traversal flow that can be used to process every element(string, list, tuple, dictionary, set) in sequence, or to execute a loop for a specified number of times. 

   Here is the syntax of a for loop:
   
   ```python
   for iterating_var in sequence:
      statements(s)
   ```

   The process flow of for loop:

   ![图片不存在](media/fa8bd2019f71f40dda2a30b803617e1b.png)

   Process strings:
   
   ```python
   # Define string name
   hopy = "reaipaobu"
   # Process the string in for loop
   for x in hopy: 
          print(x)
   ```

   Results:
   
   ```
   r
   e
   a
   i
   p
   a
   o
   b
   u
   ```
   
   In for loop, characters in the string will be output separately, so it is also called traversal loop function.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

5. ```python
   #Tone of duty cycle = 5000
   for i in a:
       buzzer.duty_u16(5000)
       buzzer.freq(i)
       time.sleep(0.2)
   ```

   Similarly, this for loop play tones when the duty cycle is 5000, each tone is played for 0.2 seconds.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, the buzzer will circularly play tones(C, D ,E, F, G, A, B) of duty cycle of 1000 and 5000. It is obvious that the sound is much louder when the duty cycle is 5000.

Click ![图片不存在](media/dc7b8f052ee9198b54f12392d91d4171.png)or click Ctrl+C to exit execution.

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

Extension

![图片不存在](media/20165af751e3a46de15eb7992240aeba.png)

Congratulations! You have played these basic notes successfully! Now let's try to compose a beautiful music and play with this passive buzzer!

Open **3.3Music.py**.

Import library to kidspico before uploading code. Open **buzzer_music.py** and choose *Upload to /*.

![图片不存在](media/baa7325b8c367b1d47fa2896a91b15b4.png)

Upload successfully.

![图片不存在](media/3b75d3d148ca10604cd90636ee952c76.png)

Click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png) to run the code. Cool! do you hear the music?

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

![图片不存在](media/4010a09457ccb90a934a457c17ece36a.png)

In this experiment, we connect the sensor to port 4. According to the board ports view, the digital io pin at port 4 is io2.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/a9a1e1a338c695e70235d62b41eb9b98.png)

Test Code

Open **3.4Humiture.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Humiture
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import Pin
import time
import dht

#Connect XHT11 sensor to pin (2)
XHT = dht.DHT11(Pin(2))

# Attain and print temperature and humidity value per seconds
while True:
    XHT.measure() # XHT11 measures a value
   # Call dht built-in function to acquire temperature and humidity values and Shell prints them
    print('temperature:',XHT.temperature(),'℃','humidity:',XHT.humidity(),'%')
    time.sleep(0.5)
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

1. `import dht`

   Import dht library to enable functions in it.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

2. `XHT = dht.DHT11(Pin(2))` 

   Connect XHT11 temperature and humidity sensor to pin io2.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

3. `XHT.measure()`
   
   Call the measure function to detect the temperature and humidity value once.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

4. `XHT.temperature()` and `XHT.humidity()`

   Call the attain function to acquire the temperature and humidity values, and then return them.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

5. `print('temperature:',XHT.temperature(),'℃','humidity:',XHT.humidity(),'%')`

   `print()` prints multiple values with a line break.

   The contents to be printed should be enclosed in single quotation marks.

   ![图片不存在](media/053cdef01438ff9456b5d0e031c4315f.png)

   And these contents must be separated with commas.

   ![图片不存在](media/1724b91ea32573d3265a91f3e1cca8f2.png)

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

6. `time.sleep(0.5)`

   Add a delay of 0.5s to refresh the values every 0.5s.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

Before uploading code, please connect wires well. Otherwise, errors will occur:

![图片不存在](media/07d0985849b07164d2eb2cc565739fc5.png)

After uploading the code, Shell prints the temperature and humidity values every 0.5s.

![图片不存在](media/664a35ec10e7acd5afe24aba0401dcd0.png)

Blow to the XHT11 sensor and you will see both temperature and humidity values rise.

![图片不存在](media/6d5d31a83e559898d281eace04285526.png)

![图片不存在](media/98743859b93bc926b824314e365e96dc.png)

Click ![图片不存在](media/dc7b8f052ee9198b54f12392d91d4171.png)or click Ctrl+C to exit execution.

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

With the change of amount of water, the voltage (0 ~ 3.3V) detected by the analog port will change accordingly. This change is continuous, which means it can be any value within 0 ~ 3.3V.

<span style="color: rgb(10, 10, 200);">The board can only process digital signals, so we need to convert analog signals in to digital ones. Thus, an ADC(Analog to Digital Converter) acquisition is required.</span>

![图片不存在](media/2fd65b883dd17bd50a77af9b5bdb37c2.png)

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

**What is ADC?**

ADC(Analog to Digital Converter) converts analog values to digital ones. The ADC acquisition is integrated in our board, so you can call it directly. 

**Kidspico ADC Parameters**

1. Reference voltage: 3.3V

1. Resolution: 12bit

   A n-bit ADC means this ADC contains 2ⁿ scales.

   12-bit ADC contains $2^{12}=4096$ scales, and it outputs totally 4096 digital values (including from 0～ 4095), each scale is $\frac{3.3}{4095}≈0.00081(V)$ 

2. General ADC input voltage calculation: 

   <font face="courier New" color="black" size=6>$ Vin= \frac {AVDD_{ADC}}{2^{Resolution Bit}-1}*ReadData$</font> 

   $AVDD_{ADC}$: Reference voltage

3. ADC channel: 5 channels

   ADC0 - ADC3 are GPIO26 - 29, among which ADC0, ADC1, ADC2 are available to commonly measure the analog voltage, while ADC3 detects on-board VSYS voltage.

   Since ADC4 is built-in, it cannot be used at the pin. It measures the value of the on-board temperature sensor.	

![图片不存在](media/1479e66a96050e577af87d5a69edab5f.png)

Modules with red housing are analog ones, so we should connect to analog io pins of the mainboard (ports with red).

![图片不存在](media/faccc06d7b4f13dbb89250282fdb20d7.png)

In this experiment, we connect the module to port 6. According to the board ports view, the analog io pin at port 6 is io28.

In addition to the measurement of water amount, this module also detects the vapor in air.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/8bbc96e5e1bfd5da77d1ab8be6bf24f0.png)

Test Code

Open **3.5Steam sensor.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Steam sensor
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import ADC  # Import ADC module
import time

# Configure ADC, range of 0-3.3V
# define io26,io27,io28,io29 to ADC channel 0,1,2,3
Water = ADC(28)  #Photores = ADC(2)
conversion_fator = 3.3 / 65535  #Voltage value of a single scale

# Read analog value every 0.1s and convert the analog value into voltage output
while True:
    Water_value = Water.read_u16()
    voltage = Water_value * conversion_fator
    print('ADC Value:',Water_value,'   Voltage:',voltage,'V')
    time.sleep(0.1)
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

1. `from machine import ADC`

   Import ADC module
   
   ![图片不存在](media/2fd65b883dd17bd50a77af9b5bdb37c2.png)
   
   **machine.ADC function**
   
   - `machine.ADC(id)`	: ADC object constructor initializes the corresponding ADC channel.
   
     id: GPIO (PIN) object (GPIO26 ~ 29) or ADC channel (0 ~ 3)
   
   - `ADC.read_u16() `	: read corresponding ADC value and return the read value.
   
     ATTENTION: <span style="color: rgb(10, 10, 200);">In MicroPython, the ADC is converted to 16-bit for calculation, that is, from 0 to 65535. This function does not directly return the value read by ADC, but the processed one, which ranges from 0 to 65535.</span>
   
     ADC voltage calculation: <font face="courier New" color="black" size=6>$ Vin= \frac {3.3*ReadData}{65535}$</font>

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

2. `Water = ADC(28)` 

   Define ADC2 to receive the analog value of the steam sensor.

   ADC0 - ADC3 are GPIO 26 - 29, among which ADC0, ADC1, ADC2 are available.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

3. `conversion_fator = 3.3 / 65535` 
   
   Voltage value of a single scale

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

4. `Water_value = Water.read_u16()`

   Read the ADC2 value of corresponding channel, and return the read value.

   `read()` reads digital inputs, while `read_u16()` reads analog inputs. `u16` indicates that the result received is not a binary (0 or 1), but an unsigned 16-bit integer (0 ~ 65535).

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

5. `voltage = Water_value * conversion_fator`

   Convert values into voltage value. The voltage value (unit: V) equals analog value multiply by the voltage value of a single scale.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, Shell outputs the detected analog values of water/vapor and the converted voltage values.

![图片不存在](media/5008b01943e34f23116070f72be96ff0.png)

The more the amount of water is / the wetter the air is, the greater the analog and voltage value will be.

![图片不存在](media/d9ff7ed5cef26927e70b130a26721c17.png)

Breath on the detection area, or touch it with a wet tissue, and you will see the analog value ans voltage will both increase.

<span style="color: rgb(2550, 10, 50);">**ATTENTION: Be careful when using water, please do not to drip to any other place outside the detection area to aviod a short circuit.**</span>

![图片不存在](media/70bb9412b1ae9bbd619e53642122c60d.png)

Click ![图片不存在](media/dc7b8f052ee9198b54f12392d91d4171.png)or click Ctrl+C to exit execution.

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

![图片不存在](media/faccc06d7b4f13dbb89250282fdb20d7.png)

In this experiment, we connect the module to port 6. According to the board ports view, the analog io pin at port 6 is io28.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/0d3c2acdcd4f134060cb9e879d489773.png)

Test Code

Open **3.6Flame sensor.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Flame sensor
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import ADC  # Import ADC module
import time

# Configure ADC, range of 0-3.3V
# Define io26,io27,io28,io29 to ADC channel 0,1,2,3
Flame = ADC(28)  #Photores = ADC(2)
conversion_fator = 3.3 / 65535  #Voltage value of a single scale

# Read analog value every 0.1s and convert the analog value into voltage output
while True:
    Flame_value = Flame.read_u16()
    voltage = Flame_value * conversion_fator
    print('ADC Value:',Flame_value,'   Voltage:',voltage,'V',end ='   ')
    if voltage < 2:
        print('Flame detected!')
    else:
        print(end ='\n')
    time.sleep(0.1)
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

The first half part is exactly the same as the previous project. In the last half, we adopt an if statement. 

Print the analog value detected by the flame sensor and the converted voltage.

When flame is detected, the voltage decrease. The brighter the flame is, the lower the voltage will be output. 

In this experiment, we set the threshold voltage value to 2 (you can modify this value according to needs), so when the voltage is lower than 2, the flame is detected.

Add an if statement to determine whether the voltage output is lower than 2.

```python
if voltage < 2:
	print('Flame detected!')
else:
    print(end ='\n')
```

If voltage < 2, Shell will display *Flame detected!* ; When voltage ≥ 2, Shell will prints values in the next line, because a line break command `end ='\n'`  is used in the code.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, *Flame detected!* will be displayed on the Shell when the flame sensor detects flame.

![图片不存在](media/f43cbd758fc084aea34e937dac557754.png)

Click ![图片不存在](media/dc7b8f052ee9198b54f12392d91d4171.png)or click Ctrl+C to exit execution.

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

![图片不存在](media/faccc06d7b4f13dbb89250282fdb20d7.png)

In this experiment, we connect the module to port 7. According to the board ports view, the analog io pin at port 7 is io27.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/618f0c3110164c8058362cbcbd1d34ba.png)

Test Code

Open **3.7Sound sensor.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Sound sensor
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import ADC
import time

# Configure ADC, range of 0-3.3V
# Define io26,io27,io28,io29 to channel 0,1,2,3
MicroPhone = machine.ADC(27)  #MicroPhone = ADC(1)
while True:
    Micro_value = MicroPhone.read_u16()
    print(Micro_value)
    time.sleep(0.1)
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**

1. Initialization. Import ADC and time module, set the pin of the sound sensor.

2. Loop.

   Read the ADC value of corresponding channel and print the value on Shell, refresh the results every 0.1s.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, speak to the MIC, and Shell will display the analog value of sound volume that is detected by the sound sensor.

![图片不存在](media/b54b854c0a3b905b79d69b92112a03b0.png)

Click ![图片不存在](media/dc7b8f052ee9198b54f12392d91d4171.png)or click Ctrl+C to exit execution.

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

<center>Comparison Table of Voltage and UV index</center>

We can have a clearly look of the UV index corresponding to the output voltage. <span style="color: rgb(10, 10, 200);">The voltage is in the unit of mV.</span>

Modules with red housing are analog ones, so we should connect to analog io pins of the mainboard (ports with red).

![图片不存在](media/faccc06d7b4f13dbb89250282fdb20d7.png)

In this experiment, we connect the module to port 8. According to the board ports view, the analog io pin at port 8 is io26.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/d10d13061c1a5040441c6450767e27b9.png)

Test Code

Open **3.8Solar ultraviolet sensor.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Solar ultraviolet sensor
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import ADC
import time

# Configure ADC, range of 0-3.3V
# Define io26,io27,io28,io29 to ADC channel 0,1,2,3
ultraviolet = ADC(26)  #ultraviolet = ADC(0)
conversion_fator = 3.3 / 65535  #Voltage value of a single scale

while True:
    ultraviolet_value = ultraviolet.read_u16()
    voltage = int(ultraviolet_value * conversion_fator * 1000)  #Convert unit into mV
    print(voltage,'mV',end = '     ')
    # voltage < 50
    if voltage < 50:
        uv = 0
    # 50 < voltage < 227
    elif voltage < 227:
        uv = 1
    # 227 < voltage < 318
    elif voltage < 318:
        uv = 2
    # 318 < voltage < 408
    elif voltage < 408:
        uv = 3
    # 408 < voltage < 503
    elif voltage < 503:
        uv = 4
    # 503 < voltage < 606
    elif voltage < 606:
        uv = 5
    # 606 < voltage < 696
    elif voltage < 696:
        uv = 6
    # 696 < voltage < 795
    elif voltage < 795:
        uv = 7
    # 795 < voltage < 881
    elif voltage < 881:
        uv = 8
    # 881 < voltage < 976
    elif voltage < 976:
        uv = 9
    # 976 < voltage < 1079
    elif voltage < 1079:
        uv = 10
    # 1079 > voltage
    else:
        uv = 11
    time.sleep(0.1)
    print('UV Index = ',uv)
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**

1. Initialization. Import ADC and time module. Connect ultraviolet sensor to pin io26 to occupy ADC channel 0.

2. Loop.

   ① Read the value of ADC0.

   ② The voltage unit in the Comparison Table is millivolt(mV), so we convert the analog value read by the sensor into voltage in mV.

   ③ **if elif** statement: set the range of UV index according to the Comparison Table.

   |    Voltage (mV)     |   UV index    |
   | :-----------------: | :-----------: |
   |   lower than 50mV   | UV index = 0  |
   |    50mV ~ 227mV     | UV index = 1  |
   |    227mV ~ 318mV    | UV index = 2  |
   |    318mV ~ 408mV    | UV index = 3  |
   |    408mV ~ 503mV    | UV index = 4  |
   |    503mV ~ 606mV    | UV index = 5  |
   |    606mV ~ 696mV    | UV index = 6  |
   |    696mV ~ 795mV    | UV index = 7  |
   |    795mV ~ 881mV    | UV index = 8  |
   |    881mV ~ 976mV    | UV index = 9  |
   |   976mV ~ 1079mV    | UV index = 10 |
   | greater than 1170mV | UV index = 11 |
   
   Determine which UV index range the converted voltage value is in, and print the result.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

1. `from machine import ADC`

   Import ADC module.

   ![图片不存在](media/2fd65b883dd17bd50a77af9b5bdb37c2.png)

   **machine.ADC function**

   - `machine.ADC(id)`	: ADC object constructor initializes the corresponding ADC channel.

     id: GPIO (PIN) object (GPIO26 ~ 29) or ADC channel (0 ~ 3)

   - `ADC.read_u16() `	: read corresponding ADC value and return the read value.

     ATTENTION: <span style="color: rgb(10, 10, 200);">In MicroPython, the ADC is converted to 16-bit for calculation, that is, from 0 to 65535. This function does not directly return the value read by ADC, but the processed one, which ranges from 0 to 65535.</span>


![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

2. `ultraviolet = ADC(26)`

   Define ADC0 to output the analog value of ultraviolet sensor.
   
   ADC0 - ADC3 are GPIO 26 - 29, among which ADC0, ADC1, ADC2 are available.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

3. `conversion_fator = 3.3 / 65535`

     Voltage value of a single scale

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

4. `ultraviolet_value = ultraviolet.read_u16()`

   Read the ADC0 value of the related channel, and assign it to ultraviolet_value.

    `read()` reads digital inputs, while `read_u16()` reads analog inputs.  `u16` indicates that the result received is not a binary (0 or 1), but an unsigned 16-bit integer (0 ~ 65535).

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

5. `voltage = int(ultraviolet_value * conversion_fator * 1000)`

   convert the read analog value into voltage in mV, and take the integer portion of the output.

   Voltage conversion formula:

   `voltage = ultraviolet_value * conversion_fator`

   The calculated voltage value is in the unit of V: 

   ![图片不存在](media/9160cbe1250f65d7cabb4f494c5c37d7.png)

   We convert it into mV by multiplying 1000, as follows:

   `voltage = ultraviolet_value * conversion_fator * 1000`

   The output: 

   ![图片不存在](media/83d81bc8b03c8a92d50cada2028b6115.png)

   Lots of decimals are remained, so we may adopt `int()` to maintain their integer portion only. `int()` converts floats into integers, which facilitate result checking. 

   Formula:

   `voltage = int(ultraviolet_value * conversion_fator * 1000)`

   Outputs:

   ![图片不存在](media/be796f82a9bfb0c82b676e2e0352cb9b.png)
   
   

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

6. ```python
   # voltage < 50
   if voltage < 50:
       uv = 0
   # 50 < voltage < 227
   elif voltage < 227:
       uv = 1
   # 227 < voltage < 318
   elif voltage < 318:
       uv = 2
   # 318 < voltage < 408
   elif voltage < 408:
       uv = 3
   # 408 < voltage < 503
   elif voltage < 503:
       uv = 4
   # 503 < voltage < 606
   elif voltage < 606:
       uv = 5
   # 606 < voltage < 696
   elif voltage < 696:
       uv = 6
   # 696 < voltage < 795
   elif voltage < 795:
       uv = 7
   # 795 < voltage < 881
   elif voltage < 881:
       uv = 8
   # 881 < voltage < 976
   elif voltage < 976:
       uv = 9
   # 976 < voltage < 1079
   elif voltage < 1079:
       uv = 10
   # 1079 < voltage
   else:
       uv = 11
   time.sleep(0.1)
   print('UV Index = ',uv)
   ```

   In this code, **if elif** statement determines the value of UV index, and Shell prints the value and refreshes every 0.1s.

   For detailed explanation of **if elif** statement, please back to part 3.2 Code Explanation.

   We set ranges according to the comparison table of voltage and UV index:

   If `voltage < 50` is True, execute `uv = 0` , so uv index is 0.
   
   If `voltage < 50` is False, skip `uv = 0` , determine whether `voltage < 227`.

   If `voltage < 227` is True, execute `uv = 1` , so uv index is 1.

   If `voltage < 227` is False, skip `uv = 1` , determine whether `voltage < 318` .

   ... ...

   If `voltage < 1079` is True, execute `uv = 10` , so uv index is 10.

   If `voltage < 1079` is False, skip `uv = 10` , execute `uv = 11` , so uv index is 11.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, Shell prints the UV index and the voltage value (mV) converted from analog values of the sensor.

![图片不存在](media/5857b3b33afb351e8c15a60031c296b2.png)

Click ![图片不存在](media/dc7b8f052ee9198b54f12392d91d4171.png)or click Ctrl+C to exit execution.

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

![图片不存在](media/b6d4df7b4d3e80f9f77b4cb361c0d9a7.png)

In this experiment, we connect the module to port 9. According to the order of the pins, the red LED is connected to pin io13, yellow to pin io14, and green to io15.

When the mainboard inputs high(1) to the module, the connected LED will light up. If it is low(0), the related LED will go off.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/539cda0fd8b40364d7baf575648d0a5f.png)

Test Code

Open **3.9Traffic light module.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Traffic light module
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import Pin
import time
 
red = Pin(13, Pin.OUT)
yellow = Pin(14, Pin.OUT)
green = Pin(15, Pin.OUT)

while True:
    #red LED lights up for 5s
    red.on()      #Red LED light
    time.sleep(5) #dalye 1s
    red.off()     #Red LED off
    
    #yellow LED blinks for 3 times
    for i in range(3):
        yellow.on()
        time.sleep(0.5)
        yellow.off()
        time.sleep(0.5)
    
    #green LED lights up for 5s
    green.on()
    time.sleep(5)
    green.off()
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

1. `red = Pin(13, Pin.OUT)`

   Connect red LED to pin io13 and set it to output. Set the yellow and green LED pins and modes.


![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

2. ```python
   #red LED lights up for 5s
   red.on()      #Red LED light
   time.sleep(5) #dalye 1s
   red.off()     #Red LED off
   ```
   
   `red.on()`  lights up the red LED.
   
   `time.sleep(1)` maintains red LED to light up for 1s.
   
   `red.off()` turns off the red LED. This part is indispensable because red will effect other colors if it is not turned off. 

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

3. ```python
   #yellow LED blinks for 3 times.
   for i in range(3):
   	yellow.on()
       time.sleep(0.5)
       yellow.off()
       time.sleep(0.5)
   ```
   
   A **for loop** is adopted here to make the yellow LED blink(on and off) for 3 times.
   
   ![图片不存在](media/2fd65b883dd17bd50a77af9b5bdb37c2.png)
   
   **range()**: creates an integer list, generally used in for loop.
   
   **Function syntax:**
   
   `range(start, stop[, step])`
   
   - start: the beginning of counting. By default, the initial value is 0. For instance, range(5) equals range(0，5)
   - stop: the ending of counting, while **stop is excluded**. For example, range(0，5) includes [0, 1, 2, 3, 4] without 5.
   - step: step is 1 by default. Again, range(0，5) can also be written as range(0, 5, 1)
   
   So, `for i in range ()` means to assign values in range to variable i in sequence.
   
   <br>
   
   **Demonstration:**
   
   `range(3)` counts from 0 to 3, including 0, 1, 2, executing three loops in total.
   
   The first loop:
   
   i = 0: yellow LED turns on for 0.5s and off for 0.5s (blinks for 1s).
   
   The second loop:
   
   i = 1: yellow LED turns on for 0.5s and off for 0.5s (blinks for 1s).
   
   The third loop:
   
   i = 2: yellow LED turns on for 0.5s and off for 0.5s (blinks for 1s).
   
   End, quit the loop.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, the red LED lights up for 5s, yellow one blinks for 3 times and green LED lights up for 5s.

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

![图片不存在](media/06a64915730e7590a0dc4dc47b722665.png)

Before using, we need to import LPS331AP.py library.

![图片不存在](media/803824b697ed82d1ec302855f39ec922.png)

Wiring Diagram

![图片不存在](media/902c8c402d34ce59ccb9a18c7e8003be.png)

Test Code

Open **3.10Air pressure detection.py**.

Upload library LPS331AP.py to kidspico first. Click it to choose *Upload to /*.

![图片不存在](media/75a6e2b957f994c4ddf299c9491efde4.png)

Upload successfully.

![图片不存在](media/f377c748f281960b8aac61c359344f30.png)

Click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Air pressure detection
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import Pin
import time
from LPS331AP import lps331ap

scl = Pin(5) 
sda = Pin(4)
bus = 0
pressure_temp = lps331ap(bus, scl, sda)
while True:
    pressure_temp.measure()
    print('pressure:',pressure_temp.pressure_data,'temperature:',pressure_temp.temp_data)
    time.sleep(0.1)
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

1. `from LPS331AP import lps331ap`
   
   Import lps331ap function.
   
   `pressure_temp.measure()` measure the pressure and temperature value once.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

2. `pressure_temp.pressure_data`
   
   attain the measured pressure value.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

3. `pressure_temp.temp_data`
   
   attain the measured temperature value.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

Before uploading the code, please ensure the wiring is connected correctly. Otherwise, errors may occur:

![图片不存在](media/e0fe70fbb42136b87101db12e8cbfa78.png)

After uploading the code, Shell outputs the pressure and temperature value and refreshes them every 0.1s.

![图片不存在](media/7a86bed14dd2a49535db921a64bf7b80.png)

Touch the sensing area with your finger, and you will see the temperature value rises.

![图片不存在](media/372d0e57149d16fdf4a529113d9b8246.png)

![图片不存在](media/0d84e8e4f9df63aaa4b5d13f20b140c0.png)

Click ![图片不存在](media/dc7b8f052ee9198b54f12392d91d4171.png)or click Ctrl+C to exit execution.

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

![图片不存在](media/eacbf0408e2f027ca8af59b05b00baca.png)

Test Code

Open **4.1Rain detection.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Rain detection
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import Pin,PWM,ADC  # Import ADC module
import time

# configure ADC, range of 0-3.3V
# define io26,io27,io28,io29 to ADC channel 0,1,2,3
Water = ADC(28)  #Water = ADC(2)
conversion_fator = 3.3 / 65535  #Voltage value of a single scale

buzzer = PWM(Pin(3))
buzzer.freq(800)

# read the analog value every 0.1s, convert the analog value into voltage output.
while True:
    Water_value = Water.read_u16()
    voltage = Water_value * conversion_fator
    print('ADC Value:',Water_value,'   Voltage:',voltage,'V')
    time.sleep(0.1)
    if voltage > 1:
        buzzer.duty_u16(5000)
    else:
        buzzer.duty_u16(0)
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**	

Set a threshold of voltage to determine the water volume. When there is too much water, the voltage exceeds the threshold, rain is detected, and the buzzer alarms. The buzzer will stop alarming when the voltage is lower than the threshold.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization. Set the pins of the steam sensor and the passive buzzer, set the voltage value of a single scale, and set the frequency of the passive buzzer.

2. Loop.

   Print the analog value and voltage of the steam sensor.
   
   Determine whether the voltage exceeds 1 (Herein, we set 1 as the threshold, which is adjustable according to needs).
   
   - voltage > 1: buzzer alarms.
   - voltage ≤ 1: buzzer does not emit sounds.

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

![图片不存在](media/5ebf8c8add33588e91805f3f2aed8916.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 7**

![图片不存在](media/6cb0a0d26e43706c6c340654c5297319.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 8**

![图片不存在](media/06698f4cfc017346049a1ca6cf920357.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Completed**

![图片不存在](media/414176f6673cde2f461c2d89b1bca116.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

Wiring Diagram

![图片不存在](media/4cd978f3613cc94a3f734448a19fa9fe.png)

Test Code

Open **4.2Fire alarm.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Fire alarm
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import Pin,PWM,ADC  # Import ADC module
import time

# configure ADC, range of 0-3.3V
# define io26,io27,io28,io29 to ADC channel 0,1,2,3
Flame = ADC(28)  #Photores = ADC(2)
conversion_fator = 3.3 / 65535  #Voltage value of a single scale

buzzer = PWM(Pin(3))
buzzer.freq(800)

# read the analog value every 0.1s, convert the analog value into voltage output.
while True:
    Flame_value = Flame.read_u16()
    voltage = Flame_value * conversion_fator
    print('ADC Value:',Flame_value,'   Voltage:',voltage,'V')
    if voltage < 2:
        buzzer.duty_u16(5000)
    else:
        buzzer.duty_u16(0)
    time.sleep(0.1)
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**

Set a threshold of voltage to determine whether there is flame. When the sensor detects flame, the voltage is lower than the threshold, and the buzzer alarms. The buzzer will stop alarming when the voltage exceeds the threshold (the sensor detects no flame).

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization. Set the pins of the flame sensor and the passive buzzer, set the voltage value of a single scale, and set the frequency of the passive buzzer.

2. Loop.

   Print the analog value and voltage of the flame sensor.

   Determine whether the voltage is lower than 2 (Herein, we set 2 as the threshold, which is adjustable according to needs).

   - voltage < 2: buzzer alarms.
   - voltage ≥ 1: buzzer does not emit sounds.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

Upload the code. When the flame sensor detects flame, the voltage will lower than 2, and the buzzer will alarm. If not, the buzzer will not emit sounds.

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

![图片不存在](media/caca86ba4ab1c99d99838e21695606e0.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Step 7**

![图片不存在](media/d8277bcc6b09ed294039ceb9cd9770ed.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

**Completed**

![图片不存在](media/3d5f8e842bda98fa7354987fc6b7b4b7.png)

![图片不存在](media/588eda85b812e0bab54badc609a31636.png)

Wiring Diagram

![图片不存在](media/2f65c76a8ea90d9c74bd5938a9722362.png)

Test Code

Open **4.3Magnetic field detection.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Magnetic field detection
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import Pin
import time

hall = Pin(8, Pin.IN)
led = Pin(11, Pin.OUT)
while True:
    value = hall.value()
    print(value, end=' ')
    if value == 0:
        led.on()
        print("A magnetic field")
    else:
        led.off()
        print("There is no magnetic field")
    time.sleep(0.1)
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**

When the Hall sensor detects a magnetic field, a low power(0) will be output, and the white LED lights up. If there is no magnetic field, high(1) will be output, and the LED goes off.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization. Set the pins of the Hall sensor and the white LED module.

2. Loop.

   Print the digital value of the power level of the Hall sensor.

   Determine whether the value equals 0 (0 means a magnetic field is detected). 

   - value = 0: the white LED lights up.
   - value ≠ 0: the white LED goes off.


![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, the Hall sensor starts to detect magnetic field.

If the sensor detects a magnetic field, the white LED will turn on. If not, the LED will go off.

![图片不存在](media/97377a5dee3ef21e6b9d98c7a1df470a.gif)

![图片不存在](media/ffabdd3c49f62391b087a8d7f7339a8c.png)

---

4.4 ThDetection

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

![图片不存在](media/39d17591577a9107339b17d0c4709c23.png)

Test Code

Open **4.4Sound detection.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Sound detection
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import ADC,Pin
import time

# configure ADC, range of 0-3.3V
# define io26,io27,io28,io29 to ADC channel 0,1,2,3
MicroPhone = machine.ADC(27)  #MicroPhone = ADC(1)

led = Pin(11, Pin.OUT)
while True:
    Micro_value = MicroPhone.read_u16()
    print(Micro_value)
    time.sleep(0.1)
    if Micro_value > 10000:
        led.on()
    else:
        led.off()
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**

Set a threshold of analog value to determine the thunder volume. When thunder is detected, the analog value exceeds the threshold, and the white LED lights up as an alarm. The LED will go off when the value is lower than the threshold.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization. Set the pins of the sound sensor and the white LED module.

2. Loop.

   Print the analog value of sound volume detected by the sound sensor.

   Determine whether the analog value is greater than 10000 (<span style="color: rgb(10, 10, 200);">Herein, we set 10000 as the standard threshold of thunder volume, which is adjustable according to needs</span>).

   - analog value > 10000, the white LED lights up.
   - analog value ≤ 10000, the white LED goes off.

![图片不存在](media/6efbaf3d2a2c7016395af93b825dea6b.png)

Test Result

![图片不存在](media/7d7e42a04d79642c6d9f614a5e61a878.png)

After uploading the code, the sound sensor detects whether there is a thunder. When the analog value of the sound exceeds 10000, a thunder is detected and the white LED will light up.

Here we stimulate thunder by playing music. When the value is greater than 10000, LED lights up.

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

![图片不存在](media/88fba009a2e032323fb7019d2b9d3a48.png)

Test Code

Open **4.5Temperature and humidity detection.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Temperature and humidity detection
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import Pin
import time
import dht

#Connect XHT11 to pin (2)
XHT = dht.DHT11(Pin(2))

red = Pin(13, Pin.OUT)
yellow = Pin(14, Pin.OUT)
green = Pin(15, Pin.OUT)

# attain temperature and humidity value per second and print them
while True:
    XHT.measure() # enable XHT11 sensor to measure the values once
   # call dht built-in function to attain tempreature value, and print it on Shell
    print('temperature:',XHT.temperature())
    time.sleep(0.1)
    if XHT.temperature() > 35:
        red.on()
        yellow.off()
        green.off()
    elif XHT.temperature() > 29:
        yellow.on()
        red.off()
        green.off()
    elif XHT.temperature() > 24:
        green.on()
        red.off()
        yellow.off() 
```

Code Explanation

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

1. Initialization. set the pins of XHT11 temperature and humidity sensor and the traffic light module.

2. Loop.

   XHT11 sensor reads and outputs the temperature values.

   Determine which section the temperature value is in, so then light up corresponding LED.

   - 24°C ≤ temperature < 29°C: the green LED lights up and other LEDs are off.
   - 29°C ≤ temperature < 35°C: the yellow LED lights up and other LEDs are off.
   - temperature > 35°C: the red LED lights up and other LEDs are off.

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

![图片不存在](media/96b761f3a8ca14e48cfc3acf436c4ede.png)

Test Code

Open **4.6Ultraviolet detection.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Ultraviolet detection
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import ADC,Pin
import time

# configure ADC, range of 0-3.3V
# define io26,io27,io28,io29 to ADC channel 0,1,2,3
ultraviolet = ADC(26)  #ultraviolet = ADC(0)
conversion_fator = 3.3 / 65535  #Voltage value of a single scale

red = Pin(13, Pin.OUT)

while True:
    ultraviolet_value = ultraviolet.read_u16()
    voltage = int(ultraviolet_value * conversion_fator * 1000)  #convert unit into mV
    print(voltage,'mV',end = '     ')
    # voltage < 50
    if voltage < 50:
        uv = 0
    # 50 < voltage < 227
    elif voltage < 227:
        uv = 1
    # 227 < voltage < 318
    elif voltage < 318:
        uv = 2
    # 318 < voltage < 408
    elif voltage < 408:
        uv = 3
    # 408 < voltage < 503
    elif voltage < 503:
        uv = 4
    # 503 < voltage < 606
    elif voltage < 606:
        uv = 5
    # 606 < voltage < 696
    elif voltage < 696:
        uv = 6
    # 696 < voltage < 795
    elif voltage < 795:
        uv = 7
    # 795 < voltage < 881
    elif voltage < 881:
        uv = 8
    # 881 < voltage < 976
    elif voltage < 976:
        uv = 9
    # 976 < voltage < 1079
    elif voltage < 1079:
        uv = 10
    # 1079 < voltage
    else:
        uv = 11
    time.sleep(0.1)
    print('uv Index = ',uv)
    if uv > 3:
        red.on()
    else:
        red.off()
```

Code Explanation

![图片不存在](media/8b7f0ae11532396b3d55b3d9e58143ad.png)

**Conceive:**

When the UV index is within 0 ~ 2, the ultraviolet light is the weakest, and it does not have much effect on the human body. When the index increases to 3 ~ 4, the ultraviolet light is weak, but remember to wear sunscreen when going out. 

Herein, we set the threshold of the UV index to 3. If the value exceeds 3, the red LED will light up to remind you to wear sunscreen. If the value does not reach 3, the LED will go off.

![图片不存在](media/2b30b20e16472c7960908a91f97928ea.png)

**Code structure:**

1. Initialization. Set the pins of the ultraviolet sensor and the traffic light module.

2. Loop.

   if elif statement to determine the range of UV index, and output the value.

   Determine whether the UV index exceeds 3.

   - UV index > 3: the red LED lights up as a reminder.
   - UV index ≤ 3: the red LED goes off.

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

![图片不存在](media/7d2df85410abf73ad08c5ca8b1e30982.png)

Test Code

Open **4.7Air pressure detection.py** and click ![图片不存在](media/bb8bff3c77c2988be0eb31c62ebefa75.png).

```python
'''
 * Filename    : Air pressure detection
 * Thonny      : Thonny 4.1.4
 * Auther      : http//www.keyestudio.com
'''
from machine import Pin
import time
from LPS331AP import lps331ap

scl = Pin(5) 
sda = Pin(4)
bus = 0
pressure_temp = lps331ap(bus, scl, sda)

red = Pin(13, Pin.OUT)
yellow = Pin(14, Pin.OUT)
green = Pin(15, Pin.OUT)
while True:
    pressure_temp.measure()
    print('pressure:',pressure_temp.pressure_data)
    time.sleep(0.1)
    if pressure_temp.pressure_data > 1050:
        red.on()
        yellow.off()
        green.off()
    elif pressure_temp.pressure_data < 950:
        yellow.on()
        red.off()
        green.off()
    elif:
        green.on()
        red.off()
        yellow.off()
```

Code Explanation

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

2. Loop.

   LPS331APTR sensor reads the air pressure value and outputs it.

   Determine which range of the pressure value is in, in order to turn of related LED.

   - air pressure > 1050hPa: the red LED lights up and other two LEDs goes off.
   - air pressure < 950hPa: the yellow LED lights up and other two LEDs goes off.
   - 950hPa < air pressure < 1050hPa: the green LED lights up and other two LEDs goes off.

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
