# Headline Event Detector

## Overview

Uses NLP tools to extract entities and features from headline data

### How It Works

This summarizer extracts parts of speech from tweet text using the spaCy NLP library's built-in 
models. 


## Application Suite

This is a testbed suite to take data from headline APIs (in this case, Google News) 
and extract event data from them. The end result of this (in progress) research project is to have an output 
of news-worthy event summaries that is generated in real-time as tweets are produced. As of now, 
this suite consists of the following applications:

* The Headline Collector
* The Feature Extractor (_this application_)
    * Uses NLP tools to extract entities and features from tweet data
* The Newsworthiness Detector
    * Compares extracted tweet features against a corpus of headlines, verified news tweets, etc., 
    using machine learning tools to detect newsworthy “events”
* The Event Dashboard
    * Shows detected events on a UI, plotting them on a map and showing them in a table in real-time