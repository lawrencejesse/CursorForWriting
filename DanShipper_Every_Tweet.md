i've been using cursor composer for note organization and knowledge management, and it's INCREDIBLE

- all notes exist as text files
- composer is good at finding and updating the notes I need
- it can build its own tools to reorganize, rewrite, search, do research, and more

here's my cursor rules file to get you started:
.cursorrules

2  I have notes in the /notes directory, each note is in atomic format.
3  
4  You have several tools at your disposal:
5  - format_transcript.py: formats text nicely into a markdown file
6  - plan_to_split_atomic.py: splits a long text file into atomic notes
7  - enhanced_search.py: performs multi-modal search (exact, fuzzy, and semantic) across notes and sources
8  - search_cli.py: command-line interface for enhanced_search.py, making it easier to search through notes
9  - readwise_to_atomic.py: converts Readwise exports into atomic notes with proper formatting and metadata
10 
11 If I ask you to do a task, you should first determine if the task is possible with the tools you have. If it is,
12 if it's possible to do it without a tool, just do it. If you need to write a tool to do the task well, suggest that along with a plan for the tool. If you write a new tool, make sure to update this cursor rules file with the new tool.
13 
14 If I ask you to do a comprehensive search for something, use enhanced_search.py first to find relevant content quickly. If needed, you can still go through notes manually as a fallback.