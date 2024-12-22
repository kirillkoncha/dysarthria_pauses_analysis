# Dysarthria and Pauses in Speech 

Dysarthria is a motor speech disorder and characterized by disruptions in respiration, laryngeal function, airflow control, and articulation, resulting in difficulties of speech quality and intelligibility.

Based on the previous literature, the presence of pauses and their characteristics, such as frequency and duration, play an important role in understanding the speech dynamics of individuals with dysarthria.

We seek to address the following questions:
+ Do individuals with dysarthria exhibit a higher frequency and duration of pauses during speech compared with healthy controls?
+ Is the intelligibility performance of dysarthria speakers positively correlated with the duration of pauses during speech?

To answer these questions, we use Nemours database of dysarthric speech (Menendez-Pidal et al., 1996). We automtically extracted every pause and its duration from the dataset.

# Repository Structure

+ **data**
  + **aggregated_file.csv** — file, which contains number of pauses and their average duration for each dataset file
  + **aggregated_participant.csv** — file, which contains average number of pauses and average duration for every participant
  + **pauses_data.csv** — file, where each line is a detected pause (with data on participant, audio file and pause duration)
+ **vis**
  + **corr_plot.png** — correlation matrix for average number of pauses, average pause duration and sentence intelligibility scores
  + **participants_averaged.png** — plots of average number of pauses and average pause duration for every participant
+ **pauses_extraction.ipynb** — notebook with code for pause extraction from the dataset
+ **speech_analysis.Rmd** — statistical analysis of the pause data

# References
X. Menendez-Pidal, J. B. Polikoff, S. M. Peters, J. E. Leonzio and H. T. Bunnell, "The Nemours database of dysarthric speech," Proceeding of Fourth International Conference on Spoken Language Processing. ICSLP '96, Philadelphia, PA, USA, 1996, pp. 1962-1965 vol.3, doi: 10.1109/ICSLP.1996.608020.

