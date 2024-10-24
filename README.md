how to use in bug bounty programs:
subfinder -d xyz.com -all  | nuclei -t crlf.yaml -rl 50
subfinder -d xyz.com -all  | nuclei -t openRedirect.yaml -rl 100
subfinder -d xyz.com -all  | nuclei -t iis.yaml
subfinder -d xyz.com -all  | nuclei -t cors.yaml -rl 100
subfinder -d xyz.com -all  | waybackurls | gf sqli | uro | nuclei -t errorsqli.yaml -rl 50
