REPORT ZTESTE01.

SELECTION-SCREEN BEGIN OF BLOCK b1 WITH FRAME.
  
          PARAMETERS: p_1bim(12) TYPE p DECIMALS 2,
                      p_2bim(12) TYPE p DECIMALS 2,
                      p_3bim(12) TYPE p DECIMALS 2,
                      p_4bim(12) TYPE p DECIMALS 2.

SELECTION-SCREEN END OF BLOCK b1.


START-OF-SELECTION.

DATA media(12) TYPE p DECIMALS 2.


media  = ( p_1bim + p_2bim + p_3bim + p_4bim ) / 4.

WRITE: 'Sua média é'.
WRITE: media.
