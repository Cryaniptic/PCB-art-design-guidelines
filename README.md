
![PCB-Layers-and-Tips-to-Optimize-PCB-Layers](https://github.com/user-attachments/assets/c23cdfcc-bad3-4d4d-9b13-6ae56803641c)
<img width="1480" height="495" alt="layer-demo" src="https://github.com/user-attachments/assets/f2438dfc-d44b-4e3b-ab29-31545c5fe0aa" />

PCB layers are specified in the design software and are intended for functional purposes.
Typically layers are used in the following manner;
 - Substrate 
	 - the physical material that everything is built on top of 
	 - usually a fiberglass weave
	 - think of it like the canvas in a painting, you cant put paint over nothing
	 - holes, slots and other cut-outs can be put on the board if you want to get interesting
 - Copper 
	 - formed on top of that substrate and then etched away to form the traces 
	 - these form the electrical connections and wires
	 - the copper layer typically has a high resolution comparatively speaking.
	 - Exposed copper is usually tinned so has a silver appearance, but depending on the process can be copper or gold colored.
	 - Exposed copper works well as highlights (Shinyyy)
 - Soldermask 
	 - is a layer pasted over the copper 
	 - it is used to prevent unwanted connections and stop solder from getting onto areas that are to be unsoldered
	 - There are gaps purposefully made in the solder mask to expose copper that we do want to solder to. 
	 - The solder mask typically has a medium resolution as it is applied in a film.
	 - Soldermask comes in a variety of colors (most commonly green), for this project it is probably going to be black or purple
	 - Soldermask does a pretty good job at covering layers underneath it, however because copper layers have a slight thickness, this creates an embossing effect, good for subtle detailing
 - Silkscreen
	 - used as an indicator layer used to designate components, provide notes and generally make the PCB more understandable
	 - Silkscreen is typically white
	 - Silkscreen has a lower resolution because it is printed on
	 - Silkscreen is quite a thick opaque layer and so has high coverage of layers under it

PCB design software generally has a workflow that revolves around these layers, so an ideal final file output would be split into the layers as follows;
 - Areas that should be filled with copper
 - Areas that are exposed (missing silkscreen, this layer works as a negative)
 - Silkscreen
