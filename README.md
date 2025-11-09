# Hadoop MapReduce Lab – Windows11 + Eclipse

**Tested:** November 9, 2025  
**OS:** Windows 11  
**IDE:** Eclipse 2025-09+  

> Original 2024 YouTube video (shared by lecturer) works on windows 10 but fails on Windows 11 due to path spaces, deprecated commands, and Eclipse package changes.

## What This Fixes
| Issue | Original (Deprecated) | Fixed (Working) |
|------|------------------------|------------------|
| Command | `hadoop fs -mkdir /input` | `hdfs dfs -mkdir /input1` |
| Path with spaces | `C:\Hadoop Data\input` | `C:\hadoop_data\input` |
| Package naming | `org.apache.hadoop.examples` | `hadoop.mapreduce.lab1` |
| Yarn startup | Fails if path has space | Use underscore paths |

## Files
- `steps-original.html` – Follows 2024 video exactly (will fail)
- `steps-renamed.html` – Renamed classes/packages + error fixes
- `output.txt` – Sample MapReduce output

## How to Use
1. Clone repo  
2. Open `steps-renamed.html` in browser  
3. Follow steps – tested on Windows 11 + Eclipse  
4. All commands use `hdfs dfs`, not `hadoop fs`

## Contact
Stuck? Email: [udaykranth01@gmail.com] 
Pull requests welcome.

---

*Credit: Based on [YouTube Video Link](https://youtu.be/htbYT7_TZKA) updated for 2025 systems.*
