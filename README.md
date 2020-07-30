Headline Event Detector
===
## Overview
The Headline Event Detector is an application that automatically ingests news headlines, 
extracts newsworthy features from them, categorizes news events from these features, 
then shares this data via a dashboard and API.

### How It Works
The Headline Event Detector contains the following jobs, each correlating with a specific 
part of the event detection process.

#### The Headline Collector
Automatically collects headlines from automated news sources and saves them to persistent 
storage for further analysis.
#### The Feature Extractor
Batch processes headlines from persistent storage in order to conduct basic natural 
language processing tasks, with an emphasis on language feature extraction.
#### The News Categorizer
Uses extracted features in order to try to categorize headlines based on a select number 
of news categories, with varying levels of importance assigned to each category. 
#### The Event Dashboard
Shows detected events in a UI that allows the user to select, filter, and parse events by 
location, time, or event type. 