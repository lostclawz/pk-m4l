PKMod 
-----
version 3 .0.0
author: Philip Kuperberg (jinxpk@gmail.com)
Midi effect that modulates any parameter in Live:

	*	Three modulation modes-
		*	Line: draw your own modulation path by clicking on the display, the curve parameter modifies the overall curve of the graph (0 = no curve). Set when the modulation restarts at the "restart" box to the right. Shift + Click removes points.
		*	Step: Simple step sequencer. Below the graph set the number of steps, how quickly to move between steps (in max time format), arrows slide the graph left and right, time ramp between steps, and curve of the ramp between steps.
		*	LFO: LFO modulation, set speed (and speed multiplier), shape, synced/free, phase, flip, low/high.
	*	The modulation mode selected will be slightly lighter than the others. You can set three parameters to modulate on the bottom right corner (first click learn and then click the parameter you
		want to modulate). Then toggle the "OFF/ON" switch to ON. PKMod will begin modulating the parameter in Live. You can set the range with the two % boxes to the left. Note when you mouse over the minimum/maximum percentage value you can see the actual minimum/maximum being passed to the parameter. If you mouse over the "LEARN" button you can read the name of the parameter the modulation is controlling. Also available on the mapping tab.

	*	The three map tabs map the modulation to the graph you draw. A diagonal line maps it into a 1-1 ratio, not changing the modulation. A diagonal line starting from the top left and going to the bottom right flips the modulation. Very slight changes can deviate the three modulations in very cool ways. This can result in subtle speed changes to enabling the modulation for only a half of the value, etc.
	*	The two boxes in the upper right corner are transformations for the modulations (applied to all three modulations).
		*	Round: First box rounds the signal (creating jagged edges), second box smooths.
			 NOTE: This also doubles as a CPU editor, if you are modulating a plugin parameter and getting insane cpu usage, turn down the second box to 0, and the first box turn up slowly from 0 to about 0.05 or 0.10. This reduces the number of messages being sent to the plugin and should reduce the cpu usage. You shouldn't need to do this when using Live's internal effects.
		*	 Smooth: Smooths the signal. Clip: Cuts off the signal on either the top or bottom and scales appropriately. Fold: First box folds the signal over itself on the bottom of the signal, the second box on the top of the signal. Wrap: First box wraps signal amount from bottom to the top, second box from top to bottom.
		*	 Jitter: Randomess, every 0-100 milliseconds (designated by the first box) we can add a random +/- percentage to the signal (designated by the second box).

	*	Max Time Formats:
		*	 4n = quarter note
		*	8n = eighth note
		*	1n = whole note
		*	16n = 16th note
		*	16nt = 16th note triplet
		*	8nd = dotted quarter note, etc.
