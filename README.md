# ShiftLeftReliability

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
