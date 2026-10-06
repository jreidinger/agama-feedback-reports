## PURPOSE

Search the internet for the feedback on Agama - SLES/openSUSE web based installer
and create report for it.

## Instructions

- PRE-REQUISITE: Before starting, always delete any existing files in this directory beside this file.
- Search for feedback on Agama or SLES/Leap/openSUSE/SUSE web based installer in the last month
- Analyze it and identify positive, negatives and suggestions for improvements
- Recognize what version it use. Leap 16.0 and SLES 16.0 share the same version (Agama 22), while Leap 16.1 and SLES 16.1 share version 24. TW uses the latest version.
- Generate a report that summarizes all positives, negatives and suggestions for improvement for each code stream.
  Report has to include resolved final links to source of such feedback so it can later checked.
  Save the generated report as a Markdown file named YYYY-MM.md where YYYY is current year and MM is current month in the current working directory
- Prioritize searching high-signal community
     hubs such as forums.opensuse.org, the r/openSUSE subreddit, and official
     SUSE/openSUSE mailing lists.
- ALWAYS perform a broader generic web search (e.g., using negative search operators `-site:...`) to capture feedback, reviews, and news from independent blogs, tech websites, and other external sources. Do not limit the search solely to the community hubs.
- EXCLUDE official documentation sites and official project blogs (e.g., `documentation.suse.com`, `susedoc.github.io`, `yast.opensuse.org`) from your analysis and report, as they represent official project resources rather than genuine user feedback.
- If a YouTube video is used as a source, keep the link in the sources list but ALWAYS append a transcription or detailed summary of the important parts of the video to the end of the report.
- Using today's current date, calculate the exact
     date range for the 'last 30 days' and restrict your search queries to that
     timeframe. Write the timeframe to report.


## Known Edge Cases

- Users sometimes refer to Agama simply as "the new YaST"
         or confuse the two. Ensure the feedback specifically references the new
         web-based installer/Agama.
- Users rarely mention exact Agama version
         numbers (like Agama 22 or Agama 24). Instruct the agent to infer the version based
         on the OS mentioned (e.g., Tumbleweed = latest, Leap 16.0 / SLES 16.0 = Agama 22, Leap 16.1 / SLES 16.1 = Agama 24).
- Search tools may return obfuscated grounding links (e.g., `vertexaisearch.cloud.google.com`).
         Instruct the agent to resolve these to their final destination URLs (e.g., using `curl -sI "<url>" | grep -i location`)
         before writing them to the report.

## Validation

- Report must list positives, negatives and suggestion for improvements
- each entry has to have link to one or more sources that is used
- each entry should contain Agama version that is used or codestream like Leap 16.0 or Leap 16.1
