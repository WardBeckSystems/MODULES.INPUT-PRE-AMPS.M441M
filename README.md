# M441M · Input Pre Amps

Ward-Beck Systems M441M, 1973|6. Wiki page: [M441M on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/PAGES/M441M.html)

| Folder | What is in it | Files |
|---|---|---|
| [SCHEMATICS/](SCHEMATICS/) | electrical drawings: schematics, functional diagrams, component layouts, wiring | 22 |
| [MECHANICAL/](MECHANICAL/) | front panels, cover plates, metalwork, assemblies; the front panel as vectors | 12 |
| [PINOUTS/](PINOUTS/) | the RTO-144 connector: connection sheets, connector layouts, rear views | 6 |
| [MANUALS/](MANUALS/) | manuals, manual pages, price lists, brochures, documents | 115 |
| [PHOTOS/](PHOTOS/) | photographs of the module | 12 |
| [SOFTWARE/](SOFTWARE/) | program listings, firmware, the plugin | 1 |
| [KICAD/](KICAD/) | KiCad schematics traced from the drawings, the symbol, PCB projects | 8 |
| [OCR/](OCR/) | the note of every file: date, origin, title block, OCR text | 59 |

<!-- module data: tools/module_specs.py, tools/forum_quotes.py -->

**On the WBSps forum (2006|39 - 2014|47):** [13 topics](FORUM.md): what owners and technicians said about it.

## Specifications

From the technical data sheet: [1973 - M441M - Channel Amplifier.pdf](MANUALS/1973%20-%20M441M%20-%20Channel%20Amplifier.pdf) page 2 (read by OCR; check against the page). As data: [`Specifications.json`](Specifications.json).

| | |
|---|---|
| **Gain** | a) Preamplifier |
| **Microphone input** | 60dB to 10dB +0.SdB selectable via sensitivity switch |
| **Line input** | unity to -l8dB +0.SaB selectable via sensitivity switch b) Booster amplifier 154B +0.25dB |
| **Frequency response** | +0.25aB 30Hz to 20kHz |
| **Noise** | Microphone input equivalent to -124 input noise for -70 sensitivity Line input greater than 75aB signal to noise (referred to a test level 10dB above the nominal operating level) |
| **Total harmonic distortion** | Less than 0.258 3 OHz to 20kHz measured with a preamplifier output level of +24aBm and a booster amplifier output level of +l8Bm |
| **Input level** | Microphone input -70dBm to-20dBm nominal -35dBm to +15dBm maximum Line Input -l0dBm to +8Bm nominal +25Bm maximum Booster amplifier input -25dBm nominal +SaBm max |
| **Source impedance** | Mi= crophone input 150 ohms balanced Line input 600 ohms or less balanced Booster amplifier input 600 ohms or less balanced. |
| **Input impedance** | Microphone input 750 ohms or greater balanced Line input 20K ohms balanced (may be externally terminated in 600 or 150 ohms) Booster amplifier input 4000 ohms balanced. |

## Circuit description

From [1973 - M441M - Channel Amplifier.pdf](MANUALS/1973%20-%20M441M%20-%20Channel%20Amplifier.pdf) pages 4-9 (read by OCR; check against the pages). As data: [`CircuitDescription.json`](CircuitDescription.json).

<details><summary>Read it</summary>

The M441M Channel Amplifier provides the following major functions:preamplification to a microphone source 8 selection of aline input sensitivity and phase reversal adjustment to either the mic or line source reverb send selection (pre or post fade) and mix control foldback select and mix control 17 shlonee eeleot_ I switch booster amplification following the mixer attenuator For the following description please refer to drawings:- B441-02-013 B181-02-001 Bl82-02-001 The microphone input is coupled through the module edge connector (pins 1 and A) to sensitivity switch SWl as in the line input coupled through bridging resistors Rl and R2 from the edge connector (pins 5 and E) to sensitivity switch Swl _ Switch decks A &amp; B of SWl provide microphone sensitivity selections from ~704BM to ~20dBm fora standard nominal output level of -l0Bm ana sensitivity selections from -loaBm to +8dBm for line inputs _ The microphone input is designed for operating from a 150 ohm source and the line input is designed to operate from a 600 ohm source or lower Both inputs are balanced to ground with the microphone input providing an input impedance of 750 ohms or greater to the source and the line input a 20K ohm bridge to the source Sensitivity adjustments made by SWl is a combination of preamplifier feed back and input pad selection _ By this means, it is possible to improve signal to noise with decreasing input sensitivity as well as maintaining the highest over all dynamic range for the channel amplifier input circuitry_ The signal output from Swl is coupled via phase reversal switch SWS to the preamplifier, input transformer Tl_ The secondary of Tl operates into I/c 21 (pins 5 and 6) This section of 7.1 is the actual preamplifierR8 and the resistors on deck C of SWl set the feedback around 21 and therefore its gain_ R3 with CRI and CR2 are an overdrive protection circuit to prevent damage to preamplifier 21 should the input to the channel amplifier be excessively overdrive _ The second section of 2l along with Q1 form an integral Low Pass Filter with components R9 = Rlo, C8 and C12 This filter has a cut-off frequency of approximately 30kHz at a rate of 12dB/octave _ This helps prevent excessively high frequency components from being passed by the system _ Cl3 couples the signal to the actively balanced power output stage of the preamplifier section 22 with Q2 and Q3 form one half of the output stage and operate in an inverting mode_ 23 with Q4 and Q5 forms the other half of the output stage and operate ina non-inverting mode. The actively balanced preamplifier output appears at pins 4 and D of the module edge connector The signal level at this point is nominally ~ lodBm and operates into the main mixer channel attenuator (normally a balanced P &amp; G 1550 slide attenuator) The mixer attenuator output operates at pins 8 and J of the channel amplifier edge connector which is the booster amplifier input (dwg _ Bl82-02-001) 2101 is connected ina configuration known as a differential cross coupled pair_ This circuit provides an actively balanced input and output with excellent longitudinal balance_ The outputs of 2101 appearing at pins 1 and 13 have their power output capability increased by the power output transistor Q101 to Q104. The balanced output signal is coupled through Clio, C1ll Llol and L102; appearing at the module edge connector pins 5 and S _ The booster amplifier output also feeds: a) the foldback level control R238 _ The output Of which passes through the foldback select switch Sw6 _ C44= C45 and summing resistors R232 and R233; appearing at pins 10 and Lab) Channel &quot;ON ' I1 switch SW4 _ with its output appearing at pins 16 and T_ c) the post position of Reverb Send Select Switch SW2 _ The preposition of Reverb Send Switch Sw2 and the input of the CUE/ Solo Switch appear at pins 7 and H of the edge connector This point is brought out separately and normally jumpered to the preamplifier output at pins 4 and D_ In the instance when an equalizer and or insert jacks are connected at the preamplifier output; then pins 7 and H would be connected at the output of the equalizer and or insert jacks. Reverb Send Switch SW2 besides providing pre-post fade selection, in addition makes selection of either Rev 1 or Rev 2 send buss These two busses appear at pins 11 and M, and 12 and N of the module connector_ (Optionally the buss selection maybe increased to 4) R219 is the Reverb Send Level controlTheoutput from the Cue/Solo select switch SW3 appears at pins 9 and K= A dc control circuit is provided with SW3 to operate an external solo relay when required_ In addition_ the Channel ON switch SW4 has additional contact closures for operating an announce turret selection ana remote control system The 48 volt supply voltage appearing at pin 22 of the module connector is decoupled through the active decoupler Q11 and Q12 to 36V Q10 senses the channel amplifier supply current by sampling the voltage developed across R49 and R50 _ Should it become excessive (greater than 100 ma) Q10 conducts reducing the drive to the base of Q12 and thereby limiting the power dissipation in the channel amplifier to a safe level_ The power supply common appears at pin V and chassis at pins 19 and W. M44lM

**AMPLIFIER**

DC Voltage Chart:

The following DC voltages are typical and may vary +108. The idle current should be between 48 ma and 52 ma with a supply voltage of 48Vdc _ The vol meter used for the following measurements should have a sensitivity of 20,000 ohms per volt or greater. Integrated_ Circuits:

Pins

8 9

12.5 24.5 22 22

**12.5 12.5 T**

12.5 12.5 22 22 24.5 13

18 36

2101

Transistors:

**COLLECTOR**

Q1 Q2 Q3 Q4 Q5 Q10 Q11 Q12 Q101 Q102 Q103 Q104 12.75 13.25 18.5 26 36 18 18 18

18.5

18 36

36.5

47.5

36.5 47.5 18 18 18.5

17.5 18.75 17.5

WB8 044im SENS 5 60 50 8 40 4 3 20 Aic OFF Vn6 REVERE

SwiB

**T / WB: 60-9**

SwIc

**JWIA**

EWZA Sw2c

SWQD sWZB OFF Pst

**PCB 182**

R23e-~

**W 4**

Ch ON

**SIDE COVER REMG VED**

USED Om MATL.

WPS Mlaan-ReCv 50, 8 Ho 4 30 = 20 Aic OFF Vn6 RFVE RE

**T / WB: 60-9**

SwIc

**3WIA**

AVc4 Pci8ZL 0 [B3B} {5]Y {z} [e {Z {Rea {Z

DJ {Bz} paZ 84J

**{BPF ~ {34 03**

TiVi

Sw IC

**D 8 049**

04} @Z {Q2 {22 {Fvs Ll Ti-6i ] Ti-RO

**{BLB? {3 {3**

B4 BxD}

Cs+3 {B} ] 8 Zi Nb 2

WL ? Ei4

Sw 3 CLE switcht_ 5 3 Wire Link Sw 3 CUE SwITCh R,s Rs 4

2.220 cwi 4

Cs 3 274 Zip Nb 4 Low 3

CLE SW switch(Wire Link SW 3 CUE SwiTch Rs.8 RS 4

**2 C**

Sw 4

7ife

</details>

<!-- /module data -->

## Photos

_Photographs of the module itself: front, back, inside, racked._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWDEta3lqN3FlTFk/view?resourcekey=0-p-0xMR9CudEprnWBCGorfg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWDEta3lqN3FlTFk&resourcekey=0-p-0xMR9CudEprnWBCGorfg" width="240" alt="1973 - M441M - wbsps - module - m441m PreAmp 001.jpg"></a><br><sub>1973|6 · wbsps - module - m441m PreAmp 001</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKX1ZMcHNudXV6aVU/view?resourcekey=0-B2GT8chYBtRTRvPARLQWfg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKX1ZMcHNudXV6aVU&resourcekey=0-B2GT8chYBtRTRvPARLQWfg" width="240" alt="1973 - M441M - wbsps - module - m441m PreAmp 002.jpg"></a><br><sub>1973|6 · wbsps - module - m441m PreAmp 002</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWExuaG5DNm5Kdjg/view?resourcekey=0-1_0f-0VqyWoK2GINxelq9A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWExuaG5DNm5Kdjg&resourcekey=0-1_0f-0VqyWoK2GINxelq9A" width="240" alt="1973 - M441M - wbsps - module - m441m PreAmp 002_small.jpg"></a><br><sub>1973|6 · wbsps - module - m441m PreAmp 002_small</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRHNpRjZOR256NUE/view?resourcekey=0-MqiM9daOn2bxll4NGF6xzg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRHNpRjZOR256NUE&resourcekey=0-MqiM9daOn2bxll4NGF6xzg" width="240" alt="1973 - M441M - wbsps - module - m441m PreAmp 003.jpg"></a><br><sub>1973|6 · wbsps - module - m441m PreAmp 003</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeXZOd3dSdEh6RHc/view?resourcekey=0-SgkAGt6i0lkvYhM41PO75w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeXZOd3dSdEh6RHc&resourcekey=0-SgkAGt6i0lkvYhM41PO75w" width="240" alt="1973 - M441M - wbsps - module - m441m PreAmp 003_small.jpg"></a><br><sub>1973|6 · wbsps - module - m441m PreAmp 003_small</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZWZvSVJjOFlhdWc/view?resourcekey=0-8A-THP_GIp01WkrW4jy2lQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZWZvSVJjOFlhdWc&resourcekey=0-8A-THP_GIp01WkrW4jy2lQ" width="240" alt="1973 - M441M - wbsps - module - m441m PreAmp 004.jpg"></a><br><sub>1973|6 · wbsps - module - m441m PreAmp 004</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUHJiV2V1ckRaQkU/view?resourcekey=0-EXzGahqcmNtr3ksyd_ZKvQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUHJiV2V1ckRaQkU&resourcekey=0-EXzGahqcmNtr3ksyd_ZKvQ" width="240" alt="1973 - M441M - wbsps - module - m441m PreAmp 004_small.jpg"></a><br><sub>1973|6 · wbsps - module - m441m PreAmp 004_small</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWXNEWjFxdXJ2Wlk/view?resourcekey=0--lvmzqguAHgPPt5bYdZmnA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWXNEWjFxdXJ2Wlk&resourcekey=0--lvmzqguAHgPPt5bYdZmnA" width="240" alt="1973 - M441M - wbsps - promo - m441m pre-amp - front_small.jpg"></a><br><sub>1973|6 · wbsps - promo - m441m pre-amp - front_small</sub></td></tr>
</table>

Shared privately on Google Drive (opens after sign-in): [1973|6 · wbsps - module - m441m PreAmp 001_small](https://drive.google.com/file/d/0B0yR0b5T78SKM1hLTzg4MDhxRG8/view?resourcekey=0-4l9xKH000pwZx8LUDtOV7w) · [1973|6 · wbsps - promo - m441m pre-amp - back_small](https://drive.google.com/file/d/0B0yR0b5T78SKQ0J3UzVNNmpBQ28/view?resourcekey=0-P2IKppNGrp2xsFBv4aX0Ag)

Not on Google Drive yet: `472px-Wbsps_-_module_-_m441m_pre-amp_-_back.jpg`

## Mechanical

_Mechanical drawings: front panels, cover plates, metalwork and hardware (-03- drawings), AutoCAD files, each with its `(EXTRACTED).svg` vectors; `<module> - front panel.svg` is the front panel as vectors._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWGVVcDlGbEgxdmc/view?resourcekey=0-qO5fV-ZLgXpPc9-Hso2--Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWGVVcDlGbEgxdmc&resourcekey=0-qO5fV-ZLgXpPc9-Hso2--Q" width="240" alt="1973 - M441M - 441-04-013 - WAAD-BECK BYSTEMS (2).jpg"></a><br><sub>1973|6 · 441-04-013 - WAAD-BECK BYSTEMS (2) · <a href="MECHANICAL/1973%20-%20M441M%20-%20441-04-013%20-%20WAAD-BECK%20BYSTEMS%20(2)%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUGxWY3RSSHVmNVE/view?resourcekey=0-lb3xf5Jt0SbTs_N1te1CqQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUGxWY3RSSHVmNVE&resourcekey=0-lb3xf5Jt0SbTs_N1te1CqQ" width="240" alt="1973 - M441M - 441-04-013 - WAAD-BECK BYSTEMS.jpg"></a><br><sub>1973|6 · 441-04-013 - WAAD-BECK BYSTEMS · <a href="MECHANICAL/1973%20-%20M441M%20-%20441-04-013%20-%20WAAD-BECK%20BYSTEMS%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/1s_gJh-sdlbwlqp8WYUcReTfrBHAkmi1c/view" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=1s_gJh-sdlbwlqp8WYUcReTfrBHAkmi1c" width="240" alt="1973 - M441M - DOC - 441-03-010 - MOD ICKD USED.png"></a><br><sub>1973|6 · DOC - 441-03-010 - MOD ICKD USED</sub></td></tr>
</table>

## Schematics

_Electrical drawings: schematics (-02-), functional diagrams (-01-), component layouts (-06-), wiring (-09-), PCB files (.pcb .dsn), and beside each scan its `(EXTRACTED).svg`: the vectors traced from it._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYTNJUHZZU1ZZb0k/view?resourcekey=0-aAN3mTDZ0SvxI16w49svnQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYTNJUHZZU1ZZb0k&resourcekey=0-aAN3mTDZ0SvxI16w49svnQ" width="240" alt="1973 - M441M - 181-06-003.jpg"></a><br><sub>1973|6 · 181-06-003 · <a href="SCHEMATICS/1973%20-%20M441M%20-%20181-06-003%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWjdteWhyQVRWMDA/view?resourcekey=0-hK3I2HN1a-cvS18XigcC1w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWjdteWhyQVRWMDA&resourcekey=0-hK3I2HN1a-cvS18XigcC1w" width="240" alt="1973 - M441M - 182-02-001 - IGEB USED.gif"></a><br><sub>1973|6 · 182-02-001 - IGEB USED</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZXRlenVlQ0VMcU0/view?resourcekey=0-GVnpAncMIieAIC3usFIsZQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZXRlenVlQ0VMcU0&resourcekey=0-GVnpAncMIieAIC3usFIsZQ" width="240" alt="1973 - M441M - 182-06-001 - MIMBEND RAD UNLESS SPECIEIED.jpg"></a><br><sub>1973|6 · 182-06-001 - MIMBEND RAD UNLESS SPECIEIED · <a href="SCHEMATICS/1973%20-%20M441M%20-%20182-06-001%20-%20MIMBEND%20RAD%20UNLESS%20SPECIEIED%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKLWUwSHllNjZaUmc/view?resourcekey=0-yUTFHMj-8Uny1AcztMUMPg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKLWUwSHllNjZaUmc&resourcekey=0-yUTFHMj-8Uny1AcztMUMPg" width="240" alt="1973 - M441M - 441-02-013 - PIN PIN PIN PIN SUF MUTE.jpg"></a><br><sub>1973|6 · 441-02-013 - PIN PIN PIN PIN SUF MUTE · <a href="SCHEMATICS/1973%20-%20M441M%20-%20441-02-013%20-%20PIN%20PIN%20PIN%20PIN%20SUF%20MUTE%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeFZWdUNoVVR3NVk/view?resourcekey=0-1SEz5HKhBZP1VdilHI2xnQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeFZWdUNoVVR3NVk&resourcekey=0-1SEz5HKhBZP1VdilHI2xnQ" width="240" alt="1973 - M441M - 441-02-013 schematic M441M.pdf"></a><br><sub>1973|6 · 441-02-013 schematic M441M</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYUNOaDZYY3dxSjQ/view?resourcekey=0-a4yn2d6u6XHhlVIyZ23Erg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYUNOaDZYY3dxSjQ&resourcekey=0-a4yn2d6u6XHhlVIyZ23Erg" width="240" alt="1973 - M441M - B 182-06-001 - PC182 - COMPONENT LAYOUT.gif"></a><br><sub>1973|6 · B 182-06-001 - PC182 - COMPONENT LAYOUT</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOFN3VE91ZVBOOHc/view?resourcekey=0-pYQsu5LaBNqPZW0BJzTzGQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOFN3VE91ZVBOOHc&resourcekey=0-pYQsu5LaBNqPZW0BJzTzGQ" width="240" alt="1973 - M441M - schematic1_assembled.gif"></a><br><sub>1973|6 · schematic1_assembled</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKa1FpMXVPdVE5R0U/view?resourcekey=0-v-eqn5yRgGa0heGwfU2NPg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKa1FpMXVPdVE5R0U&resourcekey=0-v-eqn5yRgGa0heGwfU2NPg" width="240" alt="1973 - M441M - schematic3_assembled.gif"></a><br><sub>1973|6 · schematic3_assembled</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTkplS3VHRFNfWjA/view?resourcekey=0-d6VcLPzuj-80ja6tX8avfw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTkplS3VHRFNfWjA&resourcekey=0-d6VcLPzuj-80ja6tX8avfw" width="240" alt="1973 - M441M - schematic3_assembled.jpg"></a><br><sub>1973|6 · schematic3_assembled</sub></td></tr>
</table>

## Pinouts

_Pinouts: the RTO-144 edge connector (connection sheets, connector layouts and rear views, strapping), and the pinout / connections drawings made from them. The module root `RTO.json` lists every contact._

Not on Google Drive yet: `M441M - RTO-144 Connections.pdf`

## RTO-144 pinout

22 contacts. Every contact, with where it was read: [`RTO.json`](RTO.json).

| Pin | Signal | Kind | Pair | Confidence |
|---|---|---|---|---|
| 1 | MIC IN | in | A1 + | high |
| 4 | PREAMP OUT | out | B1 + | high |
| 5 | LINE IN | in | A2 + | high |
| 8 | BOOSTER AMP IN | in | B2 + | high |
| 10 | FOLDBACK OUT | out | A3 + | high |
| 16 | SWITCHED CH ON OUT | control | A4 + | high |
| 19 | CHASSIS | ground |  | high |
| 20 | +24 V | power |  | high |
| 22 | +48 V | power |  | high |
| A | MIC IN | in | A1 - | high |
| D | PREAMP OUT | out | B1 - | high |
| E | LINE IN | in | A2 - | high |
| J | BOOSTER AMP IN | in | B2 - | high |
| L | FOLDBACK OUT | out | A3 - | high |
| T | SWITCHED CH ON OUT | control | A4 - | high |
| V | COMMON | ground |  | high |
| Y | COMMON | ground |  | high |

## Manuals and documents

_Manuals and manual pages, price lists, RTO-144 connection sheets, brochures, ads and other document scans._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTGl3WVRnN0ZVakk/view?resourcekey=0-N7_dOFDKzc4tDI2Jdp-HJQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTGl3WVRnN0ZVakk&resourcekey=0-N7_dOFDKzc4tDI2Jdp-HJQ" width="240" alt="1973 - M441M - Archived - wbsps - promo - m441m pre-amp - 001.jpg"></a><br><sub>1973|6 · Archived - wbsps - promo - m441m pre-amp - 001</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTU5XM0ZIN001dFk/view?resourcekey=0-47rqSIGj3NYeMx5j58fH8g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTU5XM0ZIN001dFk&resourcekey=0-47rqSIGj3NYeMx5j58fH8g" width="240" alt="1973 - M441M - B 44.-6.. (cut off at right) - M44.. CHANNEL ... MODULE ... (CUT OFF).gif"></a><br><sub>1973|6 · B 44.-6.. (cut off at right) - M44.. CHANNEL ... MODULE ... (CUT OFF)</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNGFBcDRIOW1UWHc/view?resourcekey=0-nH6c7vnvGnaAB5wvOJh4-Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNGFBcDRIOW1UWHc&resourcekey=0-nH6c7vnvGnaAB5wvOJh4-Q" width="240" alt="1973 - M441M - Channel Amplifier (2).pdf"></a><br><sub>1973|6 · Channel Amplifier (2)</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeC14ZGVfV2cwTlk/view?resourcekey=0-RgAXSXLVUMSx3GNPW19SpQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeC14ZGVfV2cwTlk&resourcekey=0-RgAXSXLVUMSx3GNPW19SpQ" width="240" alt="1973 - M441M - Channel Amplifier.pdf"></a><br><sub>1973|6 · Channel Amplifier</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQXNyUkxZOXVUSUU/view?resourcekey=0-mF3KmDXVGNcVw2ykfI-kZQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQXNyUkxZOXVUSUU&resourcekey=0-mF3KmDXVGNcVw2ykfI-kZQ" width="240" alt="1973 - M441M - docs-1.gif"></a><br><sub>1973|6 · docs-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYmlZNmFvN3Rzd1k/view?resourcekey=0-X7dXIbrVrDeTL-ze_IAKVQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYmlZNmFvN3Rzd1k&resourcekey=0-X7dXIbrVrDeTL-ze_IAKVQ" width="240" alt="1973 - M441M - docs-2.gif"></a><br><sub>1973|6 · docs-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSVU0dUJsMXRGd1E/view?resourcekey=0-TFswVcLNiE9cVpbaUlo2OA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSVU0dUJsMXRGd1E&resourcekey=0-TFswVcLNiE9cVpbaUlo2OA" width="240" alt="1973 - M441M - docs-3.gif"></a><br><sub>1973|6 · docs-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZ21SaGpqVEJKNms/view?resourcekey=0-gL9igEAMjIy9rBbWihuC2Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZ21SaGpqVEJKNms&resourcekey=0-gL9igEAMjIy9rBbWihuC2Q" width="240" alt="1973 - M441M - docs-4.gif"></a><br><sub>1973|6 · docs-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbEFPSWxpTFdFMEk/view?resourcekey=0-RBLk6W8V-o_6_dn9eZgFYg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbEFPSWxpTFdFMEk&resourcekey=0-RBLk6W8V-o_6_dn9eZgFYg" width="240" alt="1973 - M441M - docs-5.gif"></a><br><sub>1973|6 · docs-5</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOXFsbV84UkRVcDQ/view?resourcekey=0-EthyUGeHdRckDCu_Len08Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOXFsbV84UkRVcDQ&resourcekey=0-EthyUGeHdRckDCu_Len08Q" width="240" alt="1973 - M441M - docs-6.gif"></a><br><sub>1973|6 · docs-6</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKLXBmUGNWS0toUzA/view?resourcekey=0-3sTWfezJN5myIIwjzwWT6w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKLXBmUGNWS0toUzA&resourcekey=0-3sTWfezJN5myIIwjzwWT6w" width="240" alt="1973 - M441M - docs-7.gif"></a><br><sub>1973|6 · docs-7</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWVlPVXZ6Y2NQeXM/view?resourcekey=0-vm-vstyd2iZJaF2HFIBQjg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWVlPVXZ6Y2NQeXM&resourcekey=0-vm-vstyd2iZJaF2HFIBQjg" width="240" alt="1973 - M441M - docs-9.gif"></a><br><sub>1973|6 · docs-9</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTmg4cTB1bzZvMmM/view?resourcekey=0-tKOACqVrPNset6lFPBU-Pw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTmg4cTB1bzZvMmM&resourcekey=0-tKOACqVrPNset6lFPBU-Pw" width="240" alt="1973 - M441M - vint P1.jpg"></a><br><sub>1973|6 · vint P1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOVluczNSNUp4VEE/view?resourcekey=0-Pffp0REFYUULKP9OmBMkcw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOVluczNSNUp4VEE&resourcekey=0-Pffp0REFYUULKP9OmBMkcw" width="240" alt="1973 - M441M - vint P10.jpg"></a><br><sub>1973|6 · vint P10</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKT2JkVTZnWlFzU1U/view?resourcekey=0-e3UU6cPkgxXoUmh_V7530w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKT2JkVTZnWlFzU1U&resourcekey=0-e3UU6cPkgxXoUmh_V7530w" width="240" alt="1973 - M441M - vint P11.jpg"></a><br><sub>1973|6 · vint P11</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVG5XN1JmT3AtaE0/view?resourcekey=0-ZgE4N61WpeYccvBbIjAq4w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVG5XN1JmT3AtaE0&resourcekey=0-ZgE4N61WpeYccvBbIjAq4w" width="240" alt="1973 - M441M - vint P2.jpg"></a><br><sub>1973|6 · vint P2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMmZ1aWlQZzhiNUk/view?resourcekey=0-kGuJAX4HKMgesG1W0ElGtQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMmZ1aWlQZzhiNUk&resourcekey=0-kGuJAX4HKMgesG1W0ElGtQ" width="240" alt="1973 - M441M - vint P3.jpg"></a><br><sub>1973|6 · vint P3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKM0RzWjAtSVJFN0U/view?resourcekey=0-J8nvfBH9fQkl6XsmbwxX_w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKM0RzWjAtSVJFN0U&resourcekey=0-J8nvfBH9fQkl6XsmbwxX_w" width="240" alt="1973 - M441M - vint P4.jpg"></a><br><sub>1973|6 · vint P4</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNXpWejBjZ1RLb3c/view?resourcekey=0-9Uf_p_rjvXSJxQ12XfNCVw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNXpWejBjZ1RLb3c&resourcekey=0-9Uf_p_rjvXSJxQ12XfNCVw" width="240" alt="1973 - M441M - vint P5.jpg"></a><br><sub>1973|6 · vint P5</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTENSZFFpcVF5UzA/view?resourcekey=0-s21JLHnveFsnuKF_-AdQRA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTENSZFFpcVF5UzA&resourcekey=0-s21JLHnveFsnuKF_-AdQRA" width="240" alt="1973 - M441M - vint P6.jpg"></a><br><sub>1973|6 · vint P6</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZllWZDJ5UU1rVUk/view?resourcekey=0-DZqlU6Fr2v1o2tQf2kzFeA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZllWZDJ5UU1rVUk&resourcekey=0-DZqlU6Fr2v1o2tQf2kzFeA" width="240" alt="1973 - M441M - vint P7.jpg"></a><br><sub>1973|6 · vint P7</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKX0lEcXgtczhmanc/view?resourcekey=0-fdcJuCAkJ3P78UecvTIGYQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKX0lEcXgtczhmanc&resourcekey=0-fdcJuCAkJ3P78UecvTIGYQ" width="240" alt="1973 - M441M - vint P8.jpg"></a><br><sub>1973|6 · vint P8</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQ25NSGRRRnpVcms/view?resourcekey=0-W4R_vO3PLK88jGNseIIKrg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQ25NSGRRRnpVcms&resourcekey=0-W4R_vO3PLK88jGNseIIKrg" width="240" alt="1973 - M441M - vint P9.jpg"></a><br><sub>1973|6 · vint P9</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdGh2WUJtLVZDZUE/view?resourcekey=0-voBxWyihVybqopuKU4dPwQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdGh2WUJtLVZDZUE&resourcekey=0-voBxWyihVybqopuKU4dPwQ" width="240" alt="1973 - M441M - wbsps - module - m441m pre-amp - back.jpg"></a><br><sub>1973|6 · wbsps - module - m441m pre-amp - back</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKa0dTMDNBazR0dVk/view?resourcekey=0-VRqED7jLDPZlXjZy_jITlg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKa0dTMDNBazR0dVk&resourcekey=0-VRqED7jLDPZlXjZy_jITlg" width="240" alt="1973 - M441M - wbsps - module - m441m pre-amp - front.jpg"></a><br><sub>1973|6 · wbsps - module - m441m pre-amp - front</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNFZzVzd1dVBhaEE/view?resourcekey=0-fRjWeu2T0DOBD-viS8XACQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNFZzVzd1dVBhaEE&resourcekey=0-fRjWeu2T0DOBD-viS8XACQ" width="240" alt="1973 - M441M - wbsps - promo - m441m pre-amp - 003.jpg"></a><br><sub>1973|6 · wbsps - promo - m441m pre-amp - 003</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWm5TX0l4eGNISU0/view?resourcekey=0-6SqIuJGmOc89KSRIRcmovA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWm5TX0l4eGNISU0&resourcekey=0-6SqIuJGmOc89KSRIRcmovA" width="240" alt="1973 - M441M - wbsps - promo - m441m pre-amp - 004.jpg"></a><br><sub>1973|6 · wbsps - promo - m441m pre-amp - 004</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbk5OaFlJcG9aUEk/view?resourcekey=0-Ag-w6063GzKls-KPyTtp6A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbk5OaFlJcG9aUEk&resourcekey=0-Ag-w6063GzKls-KPyTtp6A" width="240" alt="1973 - M441M - wbsps - promo - m441m pre-amp - back.jpg"></a><br><sub>1973|6 · wbsps - promo - m441m pre-amp - back</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B9I0nu1MPkm6Z2lLNEZYQ3ZoUDQ/view?resourcekey=0-5DX4cvFxAiR-D4EmHB4zQg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B9I0nu1MPkm6Z2lLNEZYQ3ZoUDQ&resourcekey=0-5DX4cvFxAiR-D4EmHB4zQg" width="240" alt="1975 - M441M - PRICE LIST - PRICE LIST.jpg"></a><br><sub>1975|8 · PRICE LIST - PRICE LIST</sub></td></tr>
</table>

Not on Google Drive yet: `19xx - M441M - Buffalo New York.jpg`, `19xx - M441M - M 441M Channel Amplifier Instruction Manual.jpg`, `19xx - M441M - M441M.jpg`, `m441m-docs-10.gif`, `m441m-docs-8.gif`, `wbsps - module - m441m pre-amp - back.jpg`, `wbsps - promo - m441m pre-amp - 002.jpg`

## KiCad

_KiCad: a schematic (`.kicad_sch`) traced from each electrical drawing, the module symbol (`.kicad_sym`) and its PCB projects. Traced schematics are the line work only: redraw with symbols over them._

- [1973 - M441M - 441-02-013 - PIN PIN PIN PIN SUF MUTE.kicad_sch](KICAD/1973%20-%20M441M%20-%20441-02-013%20-%20PIN%20PIN%20PIN%20PIN%20SUF%20MUTE.kicad_sch)
- [1973 - M441M - 441-02-013 schematic M441M p1.kicad_sch](KICAD/1973%20-%20M441M%20-%20441-02-013%20schematic%20M441M%20p1.kicad_sch)
- [1973 - M441M - Channel Amplifier (2) p13.kicad_sch](KICAD/1973%20-%20M441M%20-%20Channel%20Amplifier%20(2)%20p13.kicad_sch)
- [1973 - M441M - Channel Amplifier (2) p5.kicad_sch](KICAD/1973%20-%20M441M%20-%20Channel%20Amplifier%20(2)%20p5.kicad_sch)
- [1973 - M441M - Channel Amplifier p13.kicad_sch](KICAD/1973%20-%20M441M%20-%20Channel%20Amplifier%20p13.kicad_sch)
- [1973 - M441M - Channel Amplifier p5.kicad_sch](KICAD/1973%20-%20M441M%20-%20Channel%20Amplifier%20p5.kicad_sch)
- [M441M.kicad_sym](KICAD/M441M.kicad_sym)
- [index.html](KICAD/index.html)

## Software

- [index.html](SOFTWARE/index.html)

---
Archive: Anthony Peter Kuzub · [WBSps.ca](https://WBSps.ca) · [WBSps.Kuzub.com](https://WBSps.Kuzub.com)
