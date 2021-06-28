### cURL notes


```bash
# CURL connection details

dennis@bethel-laptop:~$ cat curl_format
\n
|- DNS Lookup Time -------------------------------------------------------------|:     %{time_namelookup}s\n
|- DNS Lookup Time - TCP Connect -----------------------------------------------|:     %{time_connect}s\n
|- DNS Lookup Time - TCP Connect - TLS Handshake -------------------------------|:     %{time_pretransfer}s\n
|- DNS Lookup Time - TCP Connect - TLS Handshake - App Data transfer -----------|:     %{time_starttransfer}s\n
|-----------------------------Total Time ---------------------------------------|:     %{time_total}s\n


dennis@bethel-laptop:~$ curl -ks -w "@curl_format" https://www.google.com -o /dev/null

|- DNS Lookup Time -------------------------------------------------------------|:     0.013318s
|- DNS Lookup Time - TCP Connect -----------------------------------------------|:     0.063978s
|- DNS Lookup Time - TCP Connect - TLS Handshake -------------------------------|:     0.084569s
|- DNS Lookup Time - TCP Connect - TLS Handshake - App Data transfer -----------|:     0.121986s
|-----------------------------Total Time ---------------------------------------|:     0.124089s


```