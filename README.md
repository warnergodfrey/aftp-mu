# mu sample app

* Clone: `git clone git@github.com:cplee/aftp-mu.git`
* Create Pipeline: `mu pipeline up`
* Validate: `curl -s $(mu env show acceptance -f json | jq -r '.values[]|select(.key=="BASE_URL")|.value') | grep 'Automation for the People'`
