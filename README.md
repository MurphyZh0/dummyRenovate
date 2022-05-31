# reproduction
1. docker run -it renovate/renovate:latest sh
2. cd ~ && git clone https://github.com/MurphyZh0/dummyRenovate.git && cd dummyRenovate
3. export RENOVATE_CONFIG_FILE=renovate.json
4. export RENOVATE_TOKEN=Your Personal Access Token
5. export LOG_LEVEL=trace
6. renovate MurphyZh0/dummyRenovate

You will find the in the trace that renovate keep requesting to https://api.github.com/repos/whitesource/log4j-remediations/contents/base.json which takes quite long time to finish.
  
