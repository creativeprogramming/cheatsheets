title: Curl
---

Options:

    -o <file>    # --output: write to file
    -u user:pass # --user: Authentication

    -v           # --verbose
    -vv          # Even more verbose

Data options:

    -d <data>    # --data: HTTP post data
    -G           # --get: send -d data via get

Headers:

    -A <str>     # --user-agent
    
SSL:

   --cacert <file>
   --capath <dir>

   -E <cert>     # --ecrt: Client cert file
   --cert-type   # der/pem/eng

## Examples

    # Post data:
      curl -d password=x http://x.com/y

    # Auth/data:
      curl -u user:pass -d status="Hello" http://twitter.com/statuses/update.xml
   
