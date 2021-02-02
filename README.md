# aws-scripts

This project contains useful utilitie(s) for working with AWS CLI. All of these require the [AWS CLI](https://aws.amazon.com/cli/).

### Route 53 Export

**Requirements**
- Needs `jq` on the PATH
- Needs `awscli` on the PATH

The `route53-export.sh` script, taken from this [SO post](https://stackoverflow.com/a/48498598/1601182), will export a hosted zone from AWS Route 53 in BIND text format. This can be piped to a text file:
```bash
>> ./route53-export.sh example.com > example-com.zonefile.txt
```

