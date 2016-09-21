#!/bin/bash
source /home/ecopad/services/crontab_ecolab/config.sh
#echo 'Authorization: Token '$token_key

curl -X POST --data-ascii '{"function":"ecopadq.tasks.datatask.teco_spruce_pulldata","queue":"celery","args":[],"kwargs":{  },"tags": []}' http://ecolab.cybercommons.org/api/queue/run/ecopadq.tasks.datatask.teco_spruce_pulldata/.json -H Content-Type:application/json -H 'Authorization: Token '${token_key}
