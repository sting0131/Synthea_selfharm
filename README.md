# Synthea_selfharm

## This project uses Synthea (a Synthetic Patient Population Simulator) to generate a datafile with suicide behavior and self-harm cases. The information below describes how the datafile was generated. Additional information on Synthea can be found at: https://github.com/synthetichealth/synthea/tree/master 

git clone https://github.com/synthetichealth/synthea.git
cd synthea

Save synthea-with-dependencies.jar from github to synthea folder on server

java -jar synthea-with-dependencies.jar

{\Large Generate csv files for self-harm in adult cases:}
java -jar synthea-with-dependencies.jar -m self_harm -p 1000000 --exporter.csv.export true --exporter.subfolders_by_id_substring true


Created using Python version 3.11.4
