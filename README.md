### Nodirbek Makhtumov

AI/ML engineer at Netvision Telecom, Daejeon. I build computer vision that has to
run on edge hardware — NVIDIA Jetson, Hailo NPU, Raspberry Pi, Android tablets.

Most of the interesting work happens after the model trains: quantization, backbone
surgery, moving layers onto a DLA, and then measuring what the thing actually does
on the device instead of trusting the number from training. Object detection,
segmentation and real-time video, mostly.

The pinned repos are the ones worth reading. `face-recognition` has a three-way
hardware benchmark — same pipeline in Python, C++ and on an NPU, measured against
each other. `malware_classifier` is mostly a record of trying to break my own
98.95% classifier, which took about four paragraphs and worked.

Korean · English · Russian. E-7 visa, based in Korea.
