#!/bin/bash
# brew install jq

LOKALISE_TOKEN=""
AWS_ACCESS_KEY_ID=""
AWS_SECRET_ACCESS_KEY=""

while getopts ":l:a:s:" options; do        
  case "${options}" in                    # 
    l)                                    # If the option is n,
      LOKALISE_TOKEN=${OPTARG}                      # set $NAME to specified value.
      ;;
    a)                                    # If the option is t,
      AWS_ACCESS_KEY_ID=${OPTARG}                      # set $NAME to specified value.
      ;;
    s)
       AWS_SECRET_ACCESS_KEY=${OPTARG}                      # set $NAME to specified value.
      ;;     
    :)                                    # If expected argument omitted:
      echo "Error: -${OPTARG} requires an argument."
      exit 1                       # Exit abnormally.
      ;;
    *)                                    # If unknown (any other) option:
      echo "Error: Unknow argument found."
      exit 1                    # Exit abnormally.
      ;;
  esac
done

echo $LOKALISE_TOKEN
echo $AWS_ACCESS_KEY_ID
echo $AWS_SECRET_ACCESS_KEY
