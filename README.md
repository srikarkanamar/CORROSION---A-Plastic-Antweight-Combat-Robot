# CORROSION---A-Plastic-Antweight-Combat-Robot

CORROSION PLASTIC ANTWEIGHT COMBAT ROBOT DOCUMENTATION

Project Overview:

CORROSION is a 1lb plastic antweight combat robot designed and built completely from scratch to participate in the competitive combat robotics scene. The robot is a four-wheel drum spinner, a popular archetype, augmented by defensive design and weapon optimization. This document covers the entire research, design, and build process of CORROSION, as well as the groundwork for further development.

Preliminary Research and Organization:

Through joining communities and online servers, I networked and learned from veteran competitors and individuals who had gone to the global stage competing in BattleBots™, at the largest open-division scale of combat robotics (250lb). From these valuable mentors, I managed to learn troves of information that can only be learned through experience, as well as insight into modern, novel strategies fellow builders are exploring. Engaging in these forums and servers enabled me to have designs critiqued by experts in their craft and receive advice on subsequent development.

To decide on the framework of my robot, I analyzed the current competition scene with available quantitative metrics. The first source I examined was the main organizer of the United States events’ rankings for the most successful bots. These rankings were not based on subjective analysis, but rather on a scoring based on win rate scaled with the rankings of opposing bots. Interestingly, the titleholders of each year were mostly, if not all, drum spinners. This is largely thanks to the division’s rules and their implications on robot design. Because bots are prohibited from using contact weapons that are not entirely composed of 3D-printed plastics, convergent designs of large spinning masses for engagement emerged. These designs aim to circumvent plastic’s low density and strength by creating larger contact areas and higher inertia.

Defensive and more technical designs, like shell-spinners, lifters, and grabbers, are disadvantaged by the unforgiving weight restrictions, the physical properties of legal FDM plastics, and the inability to pose a strong offensive front. Drum spinners are prominent because they are highly successful, due to their robust designs, powerful offensive strategy, and simple driving. 

In another dimension of design strategy, I decided to use a 4WD belted wheel system for my bot’s drivetrain. I settled on this model after evaluating weight, cost, ease of repair, and maneuverability.

Weight + General Considerations:

Although 2WD models occupy much less weight, they often bear smaller drums and weapons, as a result of their collapsed drivetrain. Because I aimed to create a large drum spinner, I settled on 4WD. However, traditional 4WD requires 4 motors for control, subtracting additional weight for extra motors, larger batteries, and more complex electronics, from the already scarce limit of 1lb (~ 454 grams). To leverage the power of this setup, while also minimizing weight, I implemented a belted system. This entirely removes the conventional requirements and creates a resilient, fault-tolerant drivetrain. Although the two belted front wheels create a strong grip for the bot to execute strikes and evasive maneuvers, even if the belted system fails, the fault-tolerant design retains 2WD capabilities with the directly driven motors. 

Cost:

Additional brushed drive motors are one of the highest costs for my bot’s design. An expensive, fully direct-driven bot would hinder me from participating in many tournaments and would stress my tight budget. The belted system runs on polyurethane belts and small, lathed axles, both of which are highly economical.

Ease of Repair:

A higher quantity of electronics and motors creates more points of failure for the bot to encounter in the arena. Furthermore, in the pits, where competitors are only given 20 minutes to complete their repairs, additional motors and complex electronics would be more time-consuming to troubleshoot and fix. Belted drive reduces the number of actively powered elements, allowing me to prioritize repair time on more pressing matters.

Maneuverability:

I chose a 4WD over a 2WD because of the inherent gyroscopic effects created by drum-spinners. Because the weapon drums are the largest component of a bot and spin at hundreds of RPM, they generate a gyroscopic effect that makes bots tilt violently as they turn. 4WD systems are objectively better at negating gyro-effects, leveraging their wide and stable driveframes. Meanwhile, 2WD spinners are often downsized to reduce gyroscopic interference,  which is non-negotiable for my “big stick” design strategy.


Design and Part Breakdown:

Uprights:

Well-designed uprights (most commonly used term for the two parallel vertical structures that frame the entire bot) are instrumental to success. This was not only the first part I designed, but also the one most iterated upon. I designed my uprights to house all of my motors and an external shell to create an easily replaceable structure that is “hot-swappable.” Because uprights are the most structurally significant component, I decided to prioritize strength over weight savings by adding extra material in the form of higher walls and infill. After several iterations, I landed on 3 walls and 15% sparse gyroid infill.

Side Armor:

The side armor of the bot is designed to mitigate impact as much as possible. To design effectively under the weight restriction, I implemented novel design techniques to reduce deformation and failure on impact. The first design choice I made was to run both metal axles through the armor, as well as two M3s to the uprights, in order to create a stable base. I adjusted the design to be optimized for horizontal spinner bots by reducing any type of harsh angles that spinners can catch onto. By printing in an unconventional orientation, I designed armor that chips, rather than bends under high-force impacts. Deformation of the armor could destabilize my drivetrain, leading to a plethora of disadvantages across the bot. After consulting with fellow competitors, I augmented my design to contain soft curves that create geometries that vertical spinners cannot “bite”. These surfaces result in glancing hits that fail to transfer lethal energy, giving my bot the upper hand in defensive interaction. 

Wedgelets:

CORROSION’s weapon thrives when given a point to snag and transfer as much energy as possible. This common principle, shared across vertical spinner designs has led to the development of forks and wedges. These slanted components aim to slip under opposing robots, lifting them slightly at an angle, creating a perfect point on the underside of an opponent for the weapon to impart as much energy as possible. Conventionally, in non-plastic open division events, bots use small metal wedges known as “forks” to lift up opponents. However, this design doesn’t effectively translate to CORROSION’s division, as plastics are brittle and easily break under impact. In order to create an effective “ground game,” I designed wedgelets, which merge the advantages of spanning wedges and sharp forks. The wedgelets’ dense structure allows them to sustain impact and effectively dissipate forces across the frame. Their size reduces weight, but is large enough to effectively get under competitor bots. The slanted edges allow for a greater range of direction on approaches, improving the success rate of this component.  The hook-like structure at the top acts as a limiter to prevent the bot from high-centering itself on the wedgelets.

Bottom/Top Plate:

The bottom and top plates are very simple geometries composed largely of solid infill. Because both of them cover a large surface area and all of the internal electronics, I took time to design them effectively within the weight limit. The top plate is almost entirely solid, protecting the bot from overhead spinners and impacts when immobilized. The bottom plate was designed to have grates in order to help with quick inspection, but against powerful vertical spinners, it can be interchanged with a solid version. The top plate also forms the “scoop” under the high-speed weapon. Because the front of my bot has a large spinning mass, the back of CORROSION is its most vulnerable area. However, the bot’s agility should allow it to protect this region well enough to last a round.

Weapon and Design:

The weapon is the most technically designed element of the entire bot. The following is basic knowledge necessary to understand weapon geometry:

The weapon must have its center of mass centered on its rotational axis. If it is unbalanced, it will vibrate violently, break, or impart power spikes in the motor. 
The weapon’s tooth size (the length of its hooking element) dictates the amount of “bite” it gets, and the force imparted on opponents.
Concentrating mass far from the center of a spinning body generates maximum moment of inertia (therefore, power) per gram.
The bot’s weapon is the only element that is completely solid, which means optimization to save weight is paramount.
Asymmetric weapon geometries receive better bite than symmetrical geometries



The design process of CORROSION’s weapon underwent many iterations, starting with an asymmetrical design, transferring to a symmetrical design, and later becoming a hybrid of both. This weapon design is novel and is currently being pioneered among a few other builders I contacted and worked with. Here is a breakdown of all iterations:

Asymmetrical:

CORROSION’s first weapon design was an asymmetrical drum that prioritized bite. It was composed of a center unit, a long tooth, and an equally heavy counterweight. Because CORROSION’s drum profile is very wide, the single geometry extruded weapon would definitely incur severe drag and apply motor strain, even when spinning completely unobstructed. Since every gram of material at the edge costs multiple grams of counterweight material, which is closer to the spinning axis, the weapon became unreasonably heavy. Any reductions in weight would mean reducing the strength of the tooth, which was a tradeoff I wasn’t willing to accept. During this design process, I experimented with possibly adding a smaller tooth to the counterweight, an idea that sparked future development in multi-tooth strategies.

Symmetrical:

The symmetrical design was very similar to the asymmetrical design, with a single extruded profile. Two smaller teeth created a more aerodynamic spinning body, but bite and, therefore, power transfer were attenuated. The entire strategy for CORROSION’s design was creating a lethal offensive force to compensate for vulnerabilities in defense, so this idea was scrapped. During the design process, I experimented with hollowing a small portion of the center to save weight, whilst still retaining structural integrity, a concept I would later apply to my final design.

Hybrid:

My engineering strategy for this project revolved around fusing together the strengths of different approaches to create a bot that could endure complex challenges. For my final weapon design, I merged elements from the asymmetrical and symmetrical designs. I created a drum with a multiprofile setup. The teeth were essentially slightly bolstered and lengthened versions of the symmetrical design, but instead of having one extruded geometry, I created portions on each side of the central cylindrical mass. This solved the issue of bite, as each region of impact on the weapon had only one potential tooth to deliver hits. Furthermore, this reduced a significant amount of weight compared to the symmetrical design. I furthered this by porting the hollow segment approach from the symmetrical design to the final, hybrid weapon. By creating large fillets across the teeth, I created  a smooth, drag-resistant geometry that can also handle large stress concentrations on impacts. Because the shear strength of filament printed in a continuous segment is higher than the shear strength between multiple layers (held only by layer adhesion), an optimal print orientation on the profile face was chosen. 

The weapon is directly driven by a Repeat Robotics™ 2822 brushless motor, a reliable and widely used component in the antweight class. The traditional weapon axle design was scrapped for a more modular ball bearing ring design. The weapon directly interfaces with this ball bearing ring for free movement, and is internally structurally supported by an M5 shoulder bolt. I, notably, had much frustration tweaking tolerances for clearance and proper interfacing, requiring multiple prints to get right. 

Wheels/Drive:

I am using two Repeat Robotics™ Mini Brushed Mk2s to handle belted drives for the bot. In order to achieve a polished belted drive, I used two dead axles (Repeat Robotics™ Drive Axle Ants) for the passive wheels. All of the wheels have a “canal” that allows me to link them using polyurethane belting. Although at first glance the friction-based system may look subpar to tooth-driven counterparts, this system prevents motor burnout by limiting torque at the belt’s threshold. I am currently researching and developing the best tire for these wheels, with the current promising prospects being rubber sheets and O-rings. I am limited from casting tires with silicon, because all non-plastic parts must be off the shelf, according to local rulebooks.





Groundwork for Future Development and Areas to Improve:

Electronics:
Although all electronics for this build are plug-and-play, I have yet to configure them in their entirety and connect them with the bot’s active components. I will be using an ELRS radio system, which is currently gaining popularity in the builder community over legacy CC2500 systems. The newer ELRS (controlled by my Radiomaster Pocket Controller) is more accessible and easier to troubleshoot, has better range and latency specs, and is highly supported through its open-source software. I aim to experiment with the additional functionalities and presets that are available. Furthermore, I will be using open-source AM32 ESCs over older closed-source BLHELI_32s to leverage better control on the lower ends of power. 

Situational Configurations:
Although Corrosion is generally designed to handle a large variety of bot types, creating specialized configurations can improve performance. For example, against an overhead spinner, side armor is completely ineffectual, but by removing side armor, weight can be saved to repurpose by thickening and strengthening critical areas like the top plate. 

Clearance/Warping Issues:
Because of the limitations of FDM home systems, like the Bambu Lab A1 that I am currently using, thin parts and cylindrical cavities printed perpendicularly to the build plate are often subject to warping. This is attributed to the contraction of plastics as they cool, and although unavoidable, they are mitigatable. Currently, I face minimal issues, other than the rare hole that is too large to tap screws, but in hindsight, I wish I had optimized the interface points for 3D printing. At this current stage, it is unrealistic and futile to edit my entire system, but I will carry this insight into later projects and designs. 

Slicer Modifiers:
Slicers such as Bambu Studio offer simple modifiers, configurable regions where the slicer follows an alternate ruleset. This would come in handy to prioritize material and strength in higher-risk areas and reduce weight in areas that rarely come into contact with opponents. Currently, I am using part-generalized slicing, like the large majority of competitors, but this is an avenue I would like to explore. However, highly optimized builds like these are better suited for open weight classes, where modifiers can be used to alter the flex points of material like TPU. In the current PLA+ version of the bot, these changes would be largely insignificant and inconsistent for the extensive time it would take to implement.


Current Status as of March 19, 2026:

Hardware for the bot is completely finalized and polished. The bot is seven grams underweight from previous estimates, which is good news and allows for buffer weight when installing electronics. The weapon assembly is balanced, and access to new tools (electric screwdriver, precision drills, higher-quality fasteners) has sped up the development process.
