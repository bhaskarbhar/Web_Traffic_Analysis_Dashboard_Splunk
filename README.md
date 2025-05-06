# Web_Traffic_Analysis_Dashboard_Splunk

Queries Used:
index=web_logs | stats count by uri | sort -count
index=web_logs | timechart span=1h count
index=web_logs | stats count by referer | sort -count
index=web_logs | stats count by method
index=web_logs | stats count by clientip | sort -count | head 10
