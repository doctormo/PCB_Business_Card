# PCB Business Card

In this repository I will explain the steps I followed to create this Business Card made out of PCB material inspired by [Chris Tully's card from Hackaday](https://hackaday.io/cast4)

![Front](https://github.com/Hanqaqa/PCB_Business_Card/blob/master/Media/Front.jpg)
![Back](https://github.com/Hanqaqa/PCB_Business_Card/blob/master/Media/Back.jpg)

There are more pictures on the Media folder.

I have used 3 Open Source Programs in total:

* [KiCad v5.1.6](https://www.kicad.org/)
* [InkScape v1.1](https://inkscape.org/)
* [Svg2Shenzen v0.2.18.7](https://github.com/badgeek/svg2shenzhen)

The instructions are very easy and clear on how to install each program.

## Creating the Canvas in InkScape

Once the extension has been added in InkScape. Go to Extension > Svg2Shenzhen > Prepare Document and create a 100 x 100 mm document and click Apply.

Start creating your design by layers. Keep in mind how **Unexposed Copper**, **Exposed Copper**, **SilkScreen** and **Naked FR4** look like. Try to play with those combinations. [This video by TwinkleTwinkie](https://www.youtube.com/watch?v=Sbkvza8cKQE) gives a good tutorial on how the whole proccess works. He also shows a good overview of the color palette you will have:

![Color Palette](https://github.com/Hanqaqa/PCB_Business_Card/blob/master/Media/ColorPalette.PNG)

After fiddling with InkScape for a couple of hours (The GUI isn't that intuitive and I wasn't particularly inspired) I ended up with these layers:

![Final Composition](https://github.com/Hanqaqa/PCB_Business_Card/blob/master/Media/PCBLayers.png)

Disclaimer: I couldn't get to work the edge.cuts layer in InkScape ([Same problem as him](https://github.com/badgeek/svg2shenzhen/issues/119)), so since it was a simple 85.6x54 mm card with edges of 2.5 mm radius. I easily drew them in KiCad in the Edge.Cuts Layer.

## Sending the File

Once I had everything finished. I prepared my Gerber files in KiCad, packed them inside a rar and ordered them to JLCPCB with standard 0.8mm thickness and everything else with default settings, HASL with lead, FR4 base, black PCB Color... 10 of them cost me 4$ + 20$ shipping, so a bit expensive for my taste. 

In this repository you can find the [SVG file](https://github.com/Hanqaqa/PCB_Business_Card/blob/master/drawing.svg) I made in InkScape, as well as the [Gerber files](https://github.com/Hanqaqa/PCB_Business_Card/blob/master/Gerbers/Gerbers.rar) I made in KiCad and sent to JLCPCB. 
