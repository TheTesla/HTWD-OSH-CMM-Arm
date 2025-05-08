
# Arm Assembly

The core strategic asset behind open source instrumentation equipment is the adaptability. This manual shows the basic mounting concept and one possible setup of the arm mechanics. If it is built up with different dimensions, the calibration values in the firmware must be changed!

## Joints

To address the flexibility requirement, there are only a few amount of different parts, which are identical for each joint.

The optical rotary encoders are mounted into the `encodermountI_4` brick by three screws. The screws are normally included with the deilvery of the rotary encoder. There are six holes in the encoder. The three outer holes must be used. There is only one valid position, because the cable must fit into the large notch.

After the screws are tightened, the mounting brackets `notched_screwbarI_4` for the shaft can be fitted. For each encoder two identical parts are used. The notches of the two bricks will embrace the shaft of the encoder. It is easier to align the two parts without the encoder and combine them with one screw at first. There must not be any gap. The two bricks can be rotatetaround the screw like a pair of scissors. The assembly can now be put on the encoder shaft and a second screw must be added. At the end, both screws must be fully tigthened to make sure, the mounting brackets don't move on the shaft. Make sure, there are 1 - 2 mm spacing between the brackets and the three metal screws to avoid scrubbing or blocking.

One joint is ready now. Repeat this procedure for the other four joint.

## Segments

Having more than three joints allows to turn the pointer to reach the object from different directions. There are multiple different configurations possible. The following configuration is recommended to have a good combimation of ergonomy and felxibility:

The shaft of the first encoder points upwards. The whole movable part of the arm stands on it. The second encoder is mounted with an angle of 90° on the shaft. The hight is not critical. It changes only the absoulte z-position of the resulting coordinates. On that shaft, an arm segment in mounted in 90° angle. The third encoder is mounted in the same direction with 195 mm distance on that segment. The distance along the rotation axes is not critical. The foruth encoder is rotatet 90° to the third one. The position of it is critical. It rotation axis of it should intersect the rotation axis of the first (vertical) encoder. If it is out of center, the distance between these two rotation axes must be measured and used as calibration value. 

