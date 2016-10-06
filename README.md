# SecureTextfieldFail

I have found what looks like a memory leak in UITextfield.

If you copy >(w9UL0R>yL]]A&H;Z<f?WPHR&PU*WD&9+?iy7)& and paste into the textfield, you will see that the Works textfield works fine but in the fails textfield it will cause the app to crash.

Reason for failure:
Creating a secure textfield with a min font size 12 and adjust to fit enabled, but a font size of System light 17.0

The key is having a min font size less than the normal font size in a secure textfield.
