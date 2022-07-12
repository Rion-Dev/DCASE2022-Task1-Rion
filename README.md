# DCASE2022-Task1-Rion
This is a repostiory inteded the RION submission for DCASE2022 Task 1: Low-Complexity Acoustic Scene Classification.
Technical report is [here](https://dcase.community/documents/challenge2022/technical_reports/DCASE2022_Sugahara_107_t1.pdf).

## Folder Structure
    ├── TAU-urban-acoustic-scenes-2022-mobile-development      <- dataset 
    │   ├── audio                                              <- audio data
    │   ├── evaluation_setup        　　　　　                  <- file path and label    
    └── DCASE2022-Task1-Rion                                   
        ├── dockerfile                                         <- Docker file
        ├── NeSsi                                              <- Model size calculation　https://github.com/AlbertoAncilotto/NeSsi
        │── model                                              <- model
        │── reuse                                              <- input feature as numpy file
        │── main.ipynb                                         <- main code
        │── estimate_devices_freq.ipynb                        <- for spectrum modulation
        │── config_submit1.py                                  <- config file
        │── pcgrad.py                                          <- multi-task learning system https://github.com/WeiChengTseng/Pytorch-PCGrad
        │── README.md
        └── .gitignore                                         <- Specifies intentionally untracked files to ignore

