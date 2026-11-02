# half-wave-rectifier
Simple half wave rectifier
This circuit is quite simple but important to understand in order to make a AC-DC Converter. 
Using a signal generator with an internal resistance of 50 ohms (labeled as R,internal), we connect a 1N4007 diode in series to that along with
a load resistor (labeled as Rload). 
Quick explanation on how a half-wave rectifier works: The input V1 is a sine wave, an AC source, so it alternates between a negative and positive voltage. 
When the input V1 is a positive voltage (<0.6V), the diode is forward-biased and it conducts, resulting in a 0.6V voltage drop across it, resulting in peak voltage = 9.4V (10-0.6).
As the voltage drops below 0V, the diode enters the reverse-bias mode, resulting in 0 current going through it. Because of this, the voltage across R,load = 0, since V = I * R, and I = 0.
That exact behavior is why this circuit is called the half-wave rectifier: The positive portion of the AC-wave is left untouched, while the negative portion is transformed into a 0V constant until once again reaching positive voltage.

Obviously this behavior is frequency dependent. The lower the frequency, the better the rectification in this case. At 500Hz, this rectification is very clear and obviously working, while at higher frequencies the effect is less and less. 
