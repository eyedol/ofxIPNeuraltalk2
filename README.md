# ofxIPNeuraltalk2

### NeuralTalk Day walk with Voice

<iframe width="560" height="315" src="https://www.youtube.com/embed/l8PVcKT6PtQ" frameborder="0" allowfullscreen="allowfullscreen"></frame>

### NeuralTalk Night Walk With Voice

<iframe width="560" height="315" src="https://www.youtube.com/embed/-696q1Sg48Q" frameborder="0" allowfullscreen="allowfullscreen"></frame>

[`openFrameworks`][1], addon for IP Cameras using [Neuralktalk2][2] for automatic captioning. This is using the [`ofxIpVideoGrabber`][3] addon's example code. We've just modified it to read captions from neuraltalk2 and display it.

If you haven't seen this [video][4] already, go check it out.
It demenonstrates how deep learning can be used for automatic captioning based on what 
the webcam sees.

What we've done here is, instead of using a webcam attached directly to the computer, we're feeding neuraltalk2 with feeds from an IP camera. In addition to that we've added text to speech so it reads what the camera sees as well. Useful for a blind person interested in hearing what the camera sees.

This is a hack my friend and I worked on after seeing the original video demo of what neuraltalk2 can do.

We also modified neuraltalk2's `eval.lua`[5] script and so it's possible to read the image feed from the IP camera. 

# Dependencies
1. Neuraltalk2 [2]
2. Our modified version of `eval.lua` [5]
3. `sudo apt-get install libttspico0 libttspico-utils libttspico-data`
4. Ubuntu
5. `voice.sh`[6]

[1]: http://openframeworks.cc/
[2]: https://github.com/karpathy/neuraltalk2
[3]: https://github.com/bakercp/ofxIpVideoGrabber
[3]: https://vimeo.com/146492001
[4]: https://github.com/karpathy/neuraltalk2/blob/master/eval.lua
[5]: https://github.com/eyedol/ofxIPNeuraltalk2/blob/master/dependencies/eval.lua
[6]: https://github.com/eyedol/ofxIPNeuraltalk2/blob/master/dependencies/voice.sh