# WVU_CYBR_520_Group_1

https://github.com/mjahmad/CYBR520_Fall2022

Final Project

The dataset we will use is in the the following folder:

CIC_IDS_2017_Final
    -> MachineLearningCVE
        -> Friday-WorkingHours-Afternoon-DDos.pcap_ISCX

This is one dataset of a total set of logs that span a week.
(I have fixed some data errors.)
(If you download the dataset on your own you will need to contend with those issues.)

1.  Please copy my R Studio file and give it your name.
2.  Save your file in the same folder.

The file is generally too large for my PC.

At default the dataset contains 225745 obs. of 79 variables
You  can reduce that total down to 225745 obs. of 69 variables, with the following code.

only_zeros <- function(x) {
  if(class(x) %in% c("integer", "numeric")) {
    all(x == 0, na.rm = TRUE) 
  } else { 
    FALSE
  }
}

datasetNoZeroColumns <- dataset[ , !sapply(dataset, only_zeros)]

LVQ Model Finished

206 Hours, run time

I have uploaded my environment file.

You can load the environment file manually in R Studio to avoid running it yourself.
