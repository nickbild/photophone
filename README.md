# Reviving the Photophone

Believe it or not, the world's first wireless phone call was placed in 1880. I've recreated Alexander Graham Bell's photophone that made it possible, and you can too.

![](https://raw.githubusercontent.com/nickbild/photophone/refs/heads/main/media/logo.jpg)

Alexander Graham Bell will forever be known for inventing the telephone — and not much else (although he was a prolific inventor). Despite the success of the telephone, Bell considered the photophone, which he perfected four years after patenting the telephone, to be his greatest invention. He was right that wireless phones were the future, but as it turned out, the photophone was not the technology that would take us to that future.

## How It Works

### Principle of Operation

There are two main parts to a photophone, the transmitter and receiver. 

| ![](https://raw.githubusercontent.com/nickbild/photophone/refs/heads/main/media/Photophone_transmitter_4074931746_9f996df841_b.jpg) | 
|:--:| 
| *A transmitter* |

The most notable thing about the transmitter is that it contains no electronics whatsoever. A lens focuses sunlight on a flexible mirror at the end of a tube. When someone speaks into the other end of the tube, it causes the mirror to vibrate. Those vibrations, which encode the speaker’s voice, are then transmitted in the light that reflects off of the mirror.

| ![](https://raw.githubusercontent.com/nickbild/photophone/refs/heads/main/media/800px-Photophone_receiver_4074172975_288f2808f0_o.jpg) | 
|:--:| 
| *A receiver* |

At the receiver, the light from the transmitter is collected and focused by a parabolic mirror with a selenium cell at its focal point. The selenium cell was an early photoresistor, so as the level of light falling on it varied, so did its electrical resistance. Current was passed through the cell and into an electromagnetic speaker, which turned the variations back into sound.

### Shedding Some Light on the Failure

In 1880, Bell perfected the photophone and made wireless voice calls at distances of up to 700 feet. So you could call it a success, but yet this idea never took off. Why? Because the photophone used sunlight and lenses to focus light at a distance. You can only transmit just so far with this setup (this was 80 years before the laser was invented). It would also be difficult to scale, because line-of-sight needs to be maintained between all connection points, and the beams cannot cross without interfering with one another.

The work served as a predecessor to today's fiber optics, but building out an infrastructure of copper wire for the telephone proved to be simpler than a practical implementation of the photophone.

### Bringing the Photophone Back to Life

Even still, the photophone is a fascinating invention. It was so far ahead of its time, and it operated on such a clever and simple mechanism. So, I just had to recreate Bell's greatest invention, and this is how I did it.

| ![](https://raw.githubusercontent.com/nickbild/photophone/refs/heads/main/media/my_transmitter_sm.png) | 
|:--:| 
| *My transmitter* |

Above is my transmitter. It is a pill bottle attached to a tripod, with the lid removed for speaking into. The other end of the bottle was melted out with a soldering iron with an old tip. A balloon was stretched over this end to act as a flexible diaphragm. A small mirror was hot-glued to the diaphragm. When sound enters the open end of the bottle, it causes the diaphragm (and the attached mirror) to vibrate. Light being reflected off of that mirror picks up the vibrations.

| ![](https://raw.githubusercontent.com/nickbild/photophone/refs/heads/main/media/my_receiver_1_sm.png) | 
|:--:| 
| *My receiver - top* |

| ![](https://raw.githubusercontent.com/nickbild/photophone/refs/heads/main/media/my_receiver_2_sm.png) | 
|:--:| 
| *My receiver - front* |

As for the receiver, I have used a paper cup that is covered in Gorilla tape to block out ambient light. At the back, in the center, there’s a photoresistor. I have a lens that refocuses the light onto that photoresistor. 

Current passes through the photoresistor, which is in series with a 10,000 ohm resistor, and as light from the transmitter is received, the current varies. It outputs to an electromagnetic speaker — this much more modern than the one Bell used of course, and with an amplifier circuit built-in, but it operates on the same principles.

You may have noticed by now that there is just 1 lens in the build. That’s because I chose to use a laser instead of sunlight. This modern addition doesn’t change the principles of operation at all, but does let me avoid using most of the mirrors and lenses. If Bell had a laser available to him, I have no doubt he would have used it.

I have 5 volts DC running through the circuit, and one note on that — use a decent quality power supply. If it’s not a clean DC signal, you might get oscillations that distort the audio. I had that happen with cheap AC adapters.

When you have the components assembled, you just need to line them up. The laser needs to shine on the transmitter’s mirror, and that needs to reflect back to the receiver’s photoresistor. Then when sounds are made near the back of the transmitter, they will instantly be reproduced by the speaker. 

That’s it. You’ve got the world’s first wireless phone!

| ![](https://raw.githubusercontent.com/nickbild/photophone/refs/heads/main/media/circuit.png) | 
|:--:| 
| *Receiver circuit* |

| ![](https://raw.githubusercontent.com/nickbild/photophone/refs/heads/main/media/assembly_sm.png) | 
|:--:| 
| *My implementation* |

## Bill of Materials

- 1 x Photoresistor
- 1 x 10K ohm resistor
- 1 x Laser Diode — 5mW 650nm Red
- 1 x Pill bottle
- 1 x Balloon
- 1 x Small mirror
- 1 x Paper cup
- 1 x TRRS cable
- 1 x TRRS cable breakout board
- 1 x Convex lens
- 1 x Speaker
- Wires
- Gorilla tape

## About the Author

[Nick A. Bild, MS](https://nickbild79.firebaseapp.com/#!/)
