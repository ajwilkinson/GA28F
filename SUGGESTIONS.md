(original post by Nigel Pearson on diyAudio)

Very nice amp to rival 90% of designs sold retail . The bias pot is a bit too big . 470 R is usually better . Exicon MOSFET's used later on . 10N/P20 I think now .

The MOSFET gate resistors can be increased to 220R . Use standard metal film as the small inductance helps . The gates oscillate at about 5 MHz . Often 220R stops it ever showing anywhere else . The output stage will accept at least two extra MOS FET's if difficult load . Make a longer bracket and add side by side . 220R to each gate . 2 x 1 x 1/4 stock aluminum works well.

100 mA is often said to be ideal bias ( brake power line and deduct 14 mA . ie 114 mA ) . Less than that will work fine, will sound brighter . Chooses the sound you like best . Unlike bipolar transistors there isn't the more perfect point . 100 mA is the theoretical tipping point of these FET's . That is when the famed Ron is optimum . Equally setting it lower gives slightly less Ron and helps drive . It is no big deal how it is set as long as not too hot . If you can not briefly touch the MOS FET can it is too hot and may require a larger heat sink ( spit on your finger , sizzle is not a good sign ) . 0.5 degree per watt per PCB would be ideal . Less usually is OK . Do finger test when running music . Again you should just about be able to touch it ( 80 C I suspect ) . The heat sink should never be above 60 C if possible . The amps typically are about 50 % efficient all told . Techo music is 30% crest factor ( Hypex say 10% for nice music ) . So a 4R 50 watts of heat . 25 C + 30 C ambient = 55 C which is OK . For 8 R 1 deg per watt per PCB seems possible.

The 47K resistor to the input PNP transistors is said to be the worst feature of this amp . Not true . Slewing is symmetrical which is rare and good.

The 220 uF decoupling caps can be enlarged and made low Z ( 470 uF 63V ) . The 47 uF feedback arm cap can be made 63V non polar . Input cap 10 uF film type . You can take your PSU ground to between these 220 uF caps just before the output devices , it is marginally better.

27pf to 2SD756 can be NPO high grades ( most are ).

Gain can be increased to 100 using 330R and 150 uF . This will eliminate the need for a preamp . 470R will often be enough as the amp is powerful . Be careful of reducing gain . The most I tried was 15 ( 2K2 ).

The industrial FET's can be used ( IRFP etc ) . They require thermally compensated biasing like bipolar amps according to most who have done it . Purists reject this idea as they say it defeats the who idea of the Hitachi design . Dave Goodman seems to have used 100 % the Hitachi , wise man.

Make no mistake this amp will eat a Naim NAP 250 for breakfast if having a top notch PSU . It will disgrace a Quad 405 . It will please valve amp lovers . Goldmund was a similar design . HH made a 1200 watt version . It's distortion is very low especially at high frequencies . Beware fake transistors if cloning it . They will ruin it . 2SA970 2N55511/5401 might work at a pinch . HH used MPSA 42/92 which seem oddly different . Nice devices so maybe OK . The 2SD756 2SB716 are special devices of extremely high gain ( 400 on my meter ) , also low Cob . The current mirror using 1N4007 is fine as is ( excellent as proved by 3K9 balance ) . The 2 x 3K9 on the input pair collectors should balance at about 2% . 1.98 and 1.96 V often being typical ( 500 mA ) . The 100R second pair tail at 1.4 V typical ( 2 - 1.4 = 0.6 V 2SD756 bias voltage ) . I think I calculated slew rate to be 35 V/uS which is OK , it is double what it would be if a standard single VAS ( 2SD's ) . 47K is a useful input resistance if using a 10 K pot to feed it . Can be made 33K to minutely improve DC offset ( about 20 mV which is fine ).

Was also called LP 56 I think . The GA 28 was a slightly cheapened version that was 100% as good or better as used Exicon ( made in Scotland ).

Running at zero bias? (Suggestion by Nigel Wright)

Response by original Nigel:

Two Nigel's hey? Nigel says something very valuable. The special MOS FET for audio might replace germanium in a Leak amp . The germanium 0.5 V bias for two devices will be enough to drop them into the old circuit without modification ( remove drivers ) . I dare say with a little care using a scope it will be a marriage made in heaven . Exicon seem to need 1.2 V typical to do 100 mA . That means better than any silicon device even when complimentary feedback pairs ( 1.3 V ) . Dalingtons 2.5 V . I could right a page on this and not say much more . The industrial FET's might need 4 V.

The function of R9 12 K and the 6n8 poly cap is to balance the VAS's at HF . It mimics the output devices . If the voltage is changed R9 needs changing . 6.5 mA 12 K = 78 V if +/- 52 V rails . You will loose the balance in the 3K9's if wrong . Tweak until about like here . Approximately reduce the resistor exactly as the rails . Thus +/- 40 V is 9K1 . R3 is 1K / V . It would need 39K for 40 V.


johnnyx contributes this:


I found that at least 200 Ohm gate stoppers are necessary.

The Maplin MOSFET amplifier specified 100 Ohm resistors, enabled MHz oscillation in the output MOSFETs.

This oscillation eventually caused the Zobel network resistors to burn out.

I experimented to find the cause, and found that the specified gate resistors were too low, after eliminating all other options.