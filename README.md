# Video_Grep

A Subtitle Based Video Content Search Engine

- Difficulties faced
  - Playing video with seek was hard
  - Memory consumption by each SRT block was huge - had to reduce with slots
  - Not all videos had its subtitles, so had to remove files which either don't have .mp4 or .srt files
  - HTML5 supports only VTT Caption format
    - had to convert SRT to VTT

- Need Analysis
  - Do I need to do stemming?
  - Any lemmatization required?
  - Each SRT block has only 2 or 3 words. Still shall I consider this as separate document or any optimization that I can do?

- Packages Installed for this analysis:
  - pip install srt
  - pip install webvtt-py
  
- TO DO
  - Document Similarity construction
  - List view in Jupyter Note Book
  - Based on selection in listview, display video with seek
  - Remove SRT module dependency and use only WebVTT package (since it supports SRT to VTT)