# HTTP/2 Debug Log Parser
While HTTP/2 inspection is possible via Chrome's chrome://net-internals/#http2, the format of the output is an event log which details each H2 frame.    The purpose of this tool is to convert the text output from Chrome's HTTP2 event log into something that can be analyzed.

This tool can be downloaded and run as a standalone HTML page, since it has no server side dependencies except for a jquery plugin.   All of the parsing and coversion to CSV format is performed client side.   If you are unable to download the tool, then you can view it here:
http://htmlpreview.github.io/?https://github.com/pcal79/http2_debug_log_parser/blob/master/h2_debug_log_parser.html

Instructions:

1. In Google Chrome, navigate to chrome://net-internals/#http2
2. In a separate tab, load a webpage that you want to inspect HTTP/2 traffic for
3. In the net-internals tab, select the domain, and then the HTTP/2 steam
4. Click in the text event log, then use Ctrl+A to select everything on the page, and Ctrl+C to copy it to your clipboard.
5. Past the results in the first textarea field on the HTTP/2 Debug Log Parser
6. Click the "Parse HTTP/2 Debug Data" button to parse.

Once parsed, the "Generate File" button will create a downloadable CSV file that you can open in Excel for further analysis.

