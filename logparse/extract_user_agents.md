awk -F'"' '/GET/ {print $6}' access.log | sort | uniq -c | sort -rn
