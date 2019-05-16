# rita-elastic-supplement
Config files and tools for supplementing RITA findings using the Elastic Stack

Instructions for use

1.  Copy rita-logstash.conf to your logstash config directory and restart logstash to load the new config
2.  Load the rita-template.json index template file by using the Dev Tools tab in Kibana with this API command: PUT _template/rita (include the text in the file below the command) 
3.  Load the kibana-objects.json file into Kibana by using the Management > Saved Objects area and import the file
4.  Capture your RITA output to the appropriate files in /logstash ex: RITA show-beacons 20190513 >> /logstash/rita/beacon.log
5.  Use the saved searches, visualizations, and dashboard to view your RITA results
