If your car has CarPlay enabled and it is _not_ fullscreen already, [you can change that](https://www.g30-forum.de/forum/thread/684-bimmercode-expertenmodus-codierliste-und-nichts-anderes/?postID=10976#post10976):

ECU `HU_NBT_EVO` --> `3000_HMU` --> `CarPlay_Fullscreen` --> set to "aktiv"

If you have an aftermarket window tint, [you should tell your car](https://www.g30-forum.de/forum/thread/684-bimmercode-expertenmodus-codierliste-und-nichts-anderes/?postID=8474#post8474)

ECU `BDC` --> `3120 PfInternalMirror` --> set to "dunkel"

If you want you day time running lights [to also turn on the rear lights](https://www.g30-forum.de/forum/thread/309-bimmercode-liste-aller-codierungen-g30-g31/?postID=12471#post12471) (not brake lights obviously):

ECU `HU_MGU` --> `DAYDRIVING_LIGHT` --> set to "Standard" / 01
ECU `BDC_BODY3` --> `LIC_FEATURE_4` --> set to "Enable" / 01

Please note, that these options are untested. I have access to a G30 M550i pre-LCI, latest software (as of May 2021), but the second option is _not_ available.

If you want to ~kill~ make your [start-stop system](https://en.wikipedia.org/wiki/Start-stop_system) [remember your last setting](https://g30.bimmerpost.com/forums/showpost.php?p=22472406&postcount=4):

ECU `DME` --> `TCM_MSA_MEMORY` --> set to "01"

Please note that this option _might_ not be street legal in your country or jurisdiction, do this at your own risk.
