# WADE-TROSY 3.0

NMR pulse sequences and RF shapes for the experiments reported in JBNMR (2022)

Cite Reference articles @  JBNMR (2022)

The script and algorithms are patented @ https://patentcenter.uspto.gov/#!/applications/16861506

"wadetrosy_v3.0.mpp" is the WADE-NOESY pulse sequence in Bruker format. The shape files are listed below. 

|Short Name	|Full Name	|Operation Type	|Pulse Length factor	|Pulse Length	|Amplitude (B1)	|Bandwidth	|Reference|
| ----------| ----------- | ------------- | -------------       | ------------ | ----------- | ---------  |  -----|
|UA90cs1	|0.5csHN90x0.5csAz2z_rf0.00_27.125p1_bw0.91B1.mrf|WADE-90 on Amide with evol|	27.125	|27.125*50us=1356.25 us|	5 kHz|	0.91*B1	|Figure x|
|URcs1|	0.49csH180x0.49cs_rf0.00_59.000p1_bw0.44B1.mrf|	π with evol	59|	59*15us=885 us|	16.667 kHz	|0.44*B1	|Figure x|
|URcs2|	0.49csN180x0.49cs_rf0.00_22.000p1_bw0.25B1.mrf|	π with evol	|22	|22*35us = 770 us|	7.14 kHz |	0.5*B1	|Figure x|
|UARcs1|	wadeHNpix0.75cs_rf0.00_37.248p1_bw1.04B1.mrf|	WADE-180 on Amide with evol|	37.248|	37.248*50us = 1862.4 us|	5 kHz	|1.04*B1	|Figure x|
|UR1	|pix_rf0.00_7.093p1_bw0.80B1.mrf|	π	|7.093	|7.093*35us = 248.255us |	7.1429 kHz|	0.8*B1	|Figure x|
|IN2	|z2iz_rf0.00_10.021p1_bw2.40B1.mrf	|Inversion	|10.021|	10.021*12us = 12.252 us|	20.8333 kHz |	2.4*B1	|Figure x|


Bandwidth can be tuned by changing the RF power, the correponding pulse length is calculated by multiplying the 90 degree pulse length with the pulse length factor for each pulse. 

consider the 'wadepi2x_rf0.00_25.700p1_bw1.85p1.mrf' shape,

for RF amplitude 25kHz (=> 90 pulse length = 10us), pulse length = 25.7*10us = 257 us 

for RF amplitude 12.5kHz (=> 90 pulse length = 20us), pulse length = 25.7*20us = 514 us 
 

------------------------------------------------------------------------------
 

Copyright & License Statement

RF pulse shapes are copyrighted by Regents of the University of Minnesota and the software for generating RF shapes covered by US patent 11,221,384. Regents of the University of Minnesota will license the use of RF shapes solely for educational and research purposes by non-profit institutions and US government agencies only. For other proposed uses, contact umotc@umn.edu. The software may not be sold or redistributed without prior approval. One may make copies of the software for their use provided that the copies, are not sold or distributed, are used under the same terms and conditions. As unestablished research software, this code is provided on an "as is'' basis without warranty of any kind, either expressed or implied. The downloading, or executing any part of this software constitutes an implicit agreement to these terms. These terms and conditions are subject to change at any time without prior notice.
