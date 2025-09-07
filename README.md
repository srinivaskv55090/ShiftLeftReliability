# ShiftLeftReliability


How to Use This Tool (Super Simple!)
Step 1: Save the Tool

Copy the code from the box above
Open any text editor on your Mac (like TextEdit or Notes)
Paste the code
Save it as reliability-analyzer.html (make sure to change from .txt to .html)

Step 2: Open and Use

Double-click the reliability-analyzer.html file
It will open in your browser (Safari, Chrome, etc.)
That's it! The tool is now running

What You Can Do:
✅ Paste any code in the left box
✅ Choose the language (JavaScript, Python, Java, C#, SQL)
✅ Click "Analyze" or it analyzes automatically
✅ See issues instantly with suggested fixes
✅ No installation needed - runs in browser

reliabilityRules

An object keyed by language (e.g., sql, javascript, python) where each entry is an array of rules.

Each rule typically contains:

pattern: a RegExp to match (e.g. /SELECT\s+\*\s+FROM/gi)

message: short description

severity: 'error' | 'warning' | 'info'

fix: suggested remediation text

slo_impact: explanation tying the issue to SLOs

optional test function: extra check (like “only flag DELETE if there’s no WHERE”)

This is a regex-based linting approach: it finds text patterns and raises issues





JavaScript (7 rules):

Null reference crashes
Fetch without error handling
JSON.parse crashes
Long timeouts (>30s)
Infinite loops
eval() security risks
XSS via innerHTML

Python (6 rules):

File resource leaks
HTTP without timeout
Type conversion crashes
Long sleeps (>10s)
Dictionary/list bounds errors
Subprocess security risks

Java (6 rules):

NullPointerException
Unmanaged threads
Parse method crashes
File resource leaks
HTTP timeout issues
Database connection leaks

C# (6 rules):

NullReferenceException
Task.Result deadlocks
Resource disposal issues
HttpClient timeouts
Convert method crashes
Long Thread.Sleep blocks
