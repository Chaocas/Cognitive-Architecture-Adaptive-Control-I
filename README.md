# Cognitive-Architecture-Adaptive-Control-I
% This folder includes the 1st version of matlab code for the avatar

Here is the conversion code that you need to get back the linearity of your recorded time series.

load('10cmDistortion.mat');
input=idiot(end:-1:1);
[param,stat]=sigm_fit(linspace(idiot(end),idiot(1),18),idiot(end:-1:1))
Y=param(3)-(1/param(4))*log10((param(2)-param(1))./(X-param(1))-1);

X becomes the value you want to correct
Y becomes the output.
