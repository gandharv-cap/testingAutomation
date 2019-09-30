check python version
use python 2.7

`python --version`

check pip version

`python2 -m pip --version`

if not present install pip 

after installing pip 

run :

```
python2 -m pip install mysqlclient
python2 -m pip install pycrypto
python2 -m pip install pytest
python2 -m pip install requests
python2 -m pip install bson
python2 -m pip install pyasn1
python2 -m pip install pyrabbit
python2 -m pip install pymongo
python2 -m pip install bs4
python2 -m pip install thriftpy
python2 -m pip install selenium
python2 -m pip install boto3
python2 -m pip install pytest-html
python2 -m pip install pytest_ordering
python2 -m pip install lxml
```

also 

`brew install https://raw.githubusercontent.com/kadwanev/bigboybrew/master/Library/Formula/sshpass.rb`

`svn checkout https://capillary.sourcerepo.com/capillary/capquality/PlatformAutomation/platform_scripts/tunnelManager/`

`svn checkout https://capillary.sourcerepo.com/capillary/capquality/AppsAutomation/pyApps`

create var/log/capillary/tunnelManager and var/log/capillary/pyapps

comment respective line in `tunnelManager.py` and add :
`self.exeString = 'sshpass -p "<YOUR LDAP PASSWORD>" ssh -L '+str(localPort)+':'+str(values['ip'])+':'+str(values['remotePort'])+' <YOUR LDAP USERNAME>@'+Constants.jumpBox[values['cluster']]`

run startTunnel.sh inside tunnelManager

check logs for proper runs

run:

`python2 invoke.py -c nightly -m irisv2 -f test_irisV2_createCampaign_Sanity` inside pyApps
