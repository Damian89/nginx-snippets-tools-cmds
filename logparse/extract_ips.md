cat access.log | awk '{print $1}'| sort | uniq -c | sort -rn
