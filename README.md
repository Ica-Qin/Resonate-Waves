# Final Project: Resonate Waves

**Group Project -** by Peiyang Qin, Xueyi Wang, Haoqing Yan
---

## Overview

Our project Resonate Waves is an interactive music box that combines two trigger modes: one allows users to open and adjust the volume of 10 different soundtracks to create unique versions of basic music, and another will enable users to play suitable traditional Chinese instruments with two touch boards, following the basic music rhythm. With these two modes, even users who know nothing about music theory could play a pleasant sound.

Inspected by the splendid construction of the terrace farming, we decided on the theme of landscapes of waves and designed the box's appearance of mountains, clouds, water and terraces. This provides our users with an enjoyable visual and auditory experience interacting with "waves", both natural and artificial.

![hero-image](https://github.com/user-attachments/assets/829c7e4a-9309-4ad3-ba27-7e6f7b6dc8f0)



Showcase (Please open the sound)


https://github.com/user-attachments/assets/c223b157-afe8-4107-9401-a3510e9ebd4f


[codes](code)

## Roles and Responsibilities

### General
We cooperated closely and effectively together. There were some main parts that each of us took charge of while most of the works were done together with a high-quality exchange of ideas. All of us took part throughout the stages from planning, preparing, coding, prototyping, making, installation, video and photo shooting to final documentation.

### Coding
- Switches and potentiometers controlling soundtracks and volumes: Xueyi Wang
- Control of LED pixel strips to act in concert with switches and the music: Haoqing Yan
- Touch sensor and tin foil triggering VST instruments in Cubase: Peiyang Qin

Debugging and the combination of different parts of the code were done together. 

### Making
- Composition and arrangement of the background music (the 10 soundtracks): Xueyi Wang
- Design and laser cutting of mountains, clouds and trees: Haoqing Yan
- 3D modelling and printing of the terraces, box and gear construction, resin stimulating water: Peiyang Qin

Dying of the mountains, installation and other related works on making were done together.

### Documentation
- Design of the graph of sources of materials and video editing: Xueyi Wang
- Typography of showcase pages and Circuit simulation: Haoqing Yan
- Writing and Hero image: Peiyang Qin

Process recording, showcase video and photo shooting were done together.


## Plan & Preparation

### Inspiration
We started from the terraces, a very talented combination of nature and human agriculture by our ancestors, which dates back more than 2000 years in China. As a part of agriculture, possibly one of the first collective human production activities, the landscape of terraces conveys a sense of aesthetics both in its look and human wisdom. Based on this thinking, we would like to recall a feeling of appreciation for the organic combination of artificial and natural.


### Main Design Concept

To combine with the view of the terrace, we picked from the "waves": mountains, clouds and waters, and decided to use music, also a special wave, to link them with our users and convey a pleasant feeling.

### Design Decisions & Sketches
Finally, we decided that we would like to create an installation that allows users with no music theory knowledge to play with their own choice of music, with switches and touch boards. Additionally, we decided that the installation could be in the form of a music box with elements of mountains, water and terraces.

<img width="2400" height="1080" alt="composing01" src="https://github.com/user-attachments/assets/f4228b57-cd2e-4bd3-80db-2f97263c61f2" />
<img width="2400" height="1080" alt="composing02" src="https://github.com/user-attachments/assets/e33789e6-83b4-4787-b39a-dc2f4d052f53" />

## Materials and Components
**Materials**：

Acrylic boards | PLA-wood filament | UV resin | Silicone for mould-making | Kitchen foil | Glue stick | Plastic weld glue| Water-based dye

**Electronic Components**:

Arduino Mega | Arduino Leonardo | Led diode | WS2812E Full-color pixel strip | WH148 Linear taper rotary | potentiometer | Panel slide switch | Switch with hinge lever arm | 220Ω resisters

**Softwares**:
- Arduino IDE: electronic control
- Processing: soundtrack control
- Cubase: VST instrument control
- Kong Audio: Chinese instrument sound bank

<img width="2480" height="3523" alt="materials" src="https://github.com/user-attachments/assets/2ccce569-3f34-4994-835e-e904ca571c6c" />


When it comes to the fabrication industry, people always think about the aspect of pollution and waste. However, why don't we think of it as a modern form of "agriculture", simply a kind of collective production? We always blame the fabrication industry despite our intense demand for industrial goods, not only for our daily lives but also for the production of daily necessities. Just as peasants would raise fish in terraced fields to make multiple uses of the ground, we make multiple by-products in the fabrication industries as shown in the upper flow chat. We admit the truth that the fabrication industry does produce pollution and waste, but without a well-organized production system, there would be much more pollution to be produced to fulfil the growing human need brought by the development of technology.


## Working Processes

### **Sounds & Softwares**: Music composition & VST instrument preparing

Video: Music Composition (please open the sound)



https://github.com/user-attachments/assets/d6b5ff4e-9e57-4bc6-88c5-f82c257c8076





VST Instruments

<img width="1913" height="1197" alt="VSTinstrument" src="https://github.com/user-attachments/assets/60596419-6334-496e-a834-6e4d81a751df" />



As soon as we decided on the form of soundtracks and VST instrument touchboards, Xueyi started the progress of the music composition and arrangement, and Peiyang started to find the Chinese instrument sound bank. 

After weighing the limitations of the Arduino board and the 3D-printed case in handling multiple tracks against the desired musical outcome, Xueyi created a looping composition with 10 individual tracks. The overall music aligns with the project's theme, featuring a strong Chinese aesthetic. Xueyi emphasized this by using traditional instruments like the guzheng, bamboo flute, and Chinese drums. To enrich the texture of the melody, Xueyi also included plucked strings from Western orchestral instruments as a subtle background layer. 

Additionally, to give the music a bit of a "DJ vibe" (matching the first impression we wanted our project to convey), Xueyi boldly added energetic tracks featuring drum kits and synthetic percussion, which turned out quite well. 

As for the vocal elements, it's worth mentioning that both the choir and vocal samples are drawn from a traditional folk song from southern China called "Tian Hei Hei." This song reflects the blend of traditional Chinese agrarian culture with the natural environment, which perfectly fits the core concept we aimed to convey through our project.

Music Arrangement Process(Software: Garageband)



### **Programming**: Coding & Prototyping


<img width="2400" height="1080" alt="composing03" src="https://github.com/user-attachments/assets/0d1e9e9d-57be-46ce-8919-6689ebbcb62b" />

Video: Test of Switches(please open the sound)

https://github.com/user-attachments/assets/74990a7a-2599-47bb-a328-dfda76569869

Work Recordings (Please open the sound)

https://github.com/user-attachments/assets/8047db74-1ed1-4b5c-aa77-55298472d752


Video: Test of Midi(please open the sound)



https://github.com/user-attachments/assets/04684c1e-a67e-4aea-963f-7642b0c7d7f7





For controlling and playing the 10 soundtracks, we thought about using a DF player at the beginning. However, we then found that one DF player could only play one music file at a time, so we could not have the 10 soundtracks playing together but being controlled separately. When considering using 10 DF players to control the soundtracks, we were suggested using processing to control and play the sounds on the computer to cut down the cost.

We also met a laughable problem when we tried to set up the LED pixel strips. For more than 2 hours, we tried so hard to light up the pixels in the most simple way to check why it did not work, after which we found that it was simply because the first pixel on the strip we bought was broken.

The material we used for the touchboards was a lucky coincidence. We noticed one role of tinfoil when we were finding switches in the CCI building and we were about to leave when the idea suddenly came to all of us at the same time that it could be really good material for us to link to a touch sensor.



### **Physical Making**: Laser cutting, 3D printing & Resin making

After we decided to use acrylic to make the mountains, clouds and trees, Haoqing began to draw them in Adobe AI and went to the fabrication workshop for laser cutting. 

![laser-cutting](https://github.com/user-attachments/assets/f0b8d519-9473-4b2e-86fc-72148c12e6eb)


We then tried different ways to dye the mountains. The first try was using resin to make a colour layer on top of the mountain, but we then found that it did not look that good when put together with the LED pixel strips. 


After a tough search on Amazon, we decided to try water-based dyes for wood and clothes. We were so happy that it came out that they did work.

![dying-outcome](https://github.com/user-attachments/assets/c572fe39-e126-4565-ad75-b48466534c52)


![3D-models](final-project-files/pictures/3Dmodels.png)

When the laser cutting of the mountains, clouds and trees was done, Peiyang began to build the 3D models and 3D printed the box, internal structures of switches, terraces and supporting parts.

![3dmodeling](https://github.com/user-attachments/assets/e1b8a6ef-5704-4477-af40-879ad20dd4d4)
![3dpringting](https://github.com/user-attachments/assets/8fcebc4f-5177-432f-ae25-0b42f18c3a39)



The water layer on top of the terrace was made in the process of 3D printing, silicone moulds, and epoxy resin making. We first tried a PVC board, heating it to stimulate water and using epoxy resin to cover the shape, but we failed to take the resin off the PVC board so we decided quickly to do 3D printing and silicone moulds.



![epoxy-resin](https://github.com/user-attachments/assets/c170cdee-ca10-4b90-b84c-c13f9c2aa693)



The terraces were coloured with acrylic paint and epoxy resin. They were then glued with the printed racks to work with the gears on the potentiometers, allowing our users to adjust the "height" of the terraces while changing the volume of each soundtrack.

![terraces-colour](https://github.com/user-attachments/assets/f9800497-a470-4776-9608-0948eb9e3553)


### **Soldering & Installation**

In the beginning, we decided to link the LED diodes with the switches so that we do not need to control the diodes separately with additional codes. 

![circut-sketch](https://github.com/user-attachments/assets/50915ed2-2678-438c-b503-2e54d54c709d)


But when we finished the soldering process we found that this slight difference with our prototype caused a big problem to our codes. So we removed the soldering and designed the circuits again.


![final-circut](https://github.com/user-attachments/assets/c9a309e9-bfeb-4cb8-b1b0-1dd048f935a2)
<img width="2400" height="1080" alt="composing04" src="https://github.com/user-attachments/assets/180c6937-a122-457a-a3bb-051423306d26" />


## Further Development

Since we need to use Processing to control the soundtracks and VST instruments on the computer, this box should be linked with two computers to run. For further development maybe we could try other operating systems, maybe  Raspberry Pi, to make it run independently.

Group Photo(Haoqing Yan, Peiyang Qin, Xueyi Wang
![Group photo](final-project-files/pictures/group-photo.jpg)
