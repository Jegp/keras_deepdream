# Keras-based Deepdream experiment
<img src="https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000"/><br/>

See also: https://github.com/google/deepdream<br/>

This experiments (which is a work in progress) is based on some suggestions provided by the Deepdream team in this [blog post](http://googleresearch.blogspot.ch/2015/06/inceptionism-going-deeper-into-neural.html) but works in a slightly different way. I use a Gassian Pyramid and average the rescaled results of a layer with the next one. A total variation loss could be employed too, but after some experiments, I've prefered to remove it because of its blur effect.

## Requirements
<ul>
<li>Python 2.7-3.5</li>
<li>Keras</li>
<li>Theano/Tensorflow</li>
<li>SciPy</li>
<li>Scikit-Image</li>
</ul>

## Examples
(With different settings in terms of layers and number of iterations)
<table width="100%" align="center">
<tr>
<td width="auto">
<p align="center">
<img src="https://s3-us-west-2.amazonaws.com/keras-deepdream-demo/berlin_dream.jpg" align="center" height="300" width="400">
</p>
<p align="center"><b>Berlin</b></p>
</td>
<td width="auto">
<p align="center">
<img src="https://s3-us-west-2.amazonaws.com/keras-deepdream-demo/berlin_dream_3.jpg" align="center" height="300" width="400">
</p>
<p align="center"><b>Berlin</b></p>
</td>
</tr>
<tr>
<td width="auto">
<p align="center">
<img src="https://s3-us-west-2.amazonaws.com/keras-deepdream-demo/cinque_terre_dream.jpg" align="center" height="300" width="400">
</p>
<p align="center"><b>Cinque Terre</b></p>
</td>
<td width="auto">
<p align="center">
<img src="https://s3-us-west-2.amazonaws.com/keras-deepdream-demo/rome_dream.jpg" align="center" height="300" width="400">
</p>
<p align="center"><b>Rome</b></p>
</td>
</tr>
</table>

