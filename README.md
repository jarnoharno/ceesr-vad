# ceesr-vad

Julia implementation of the significant audio event detection parts of CeeSR.

## Prerequisites

You'll need julia 0.3 or higher. To install required julia packages, run

    $ julia install-deps.jl
   
## Usage

Classification accuracy can be tested from command line with

    $ ./ceesr-vad <audio_file> <label_file>
  
e.g.

    $ ./ceesr-vad ~/hiit/data/ceesr/audio/g/gi.{flac,txt}
    
    ==Confusion matrix==  predicted
                          significant  insignificant
    actual   significant  0.230        0.062
           insignificant  0.002        0.706
   
    ==Classification metrics==
    accuracy:  0.936
    precision: 0.992
    f1-score:  0.877
