## Temp change the default Python version

ln -s -f /usr/local/bin/python3 /usr/local/bin/python

## Change default Python version

echo "alias python=/usr/local/bin/python3" >> ~/.bashrc
echo "alias python=/usr/local/bin/python3" >> ~/.zshrc

echo "alias pip=/usr/local/bin/pip3" >> ~/.bashrc
echo "alias pip=/usr/local/bin/pip3" >> ~/.zshrc

- Make sure to change the default Python version to match the one used by Azure
- Make sure run pip to install those libs required by Azure function, so we can test locally

## If it is failed to run locally, solve the Python SSL issue

sudo /Applications/"Python 3.11"/"Install Certificates.command"
