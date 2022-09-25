# Grafana 

Grafana is an open-source platform for observability,running analytics and monitoring our systems online. 

## Try out Grafana Cloud on macOS

1. Register account on https://grafana.com/products/cloud/, follow the instruction
2. Follow easy set up for macOS via https://kencho.grafana.net/a/grafana-easystart-app/macos-node

3. Configuration
```
# 1. Choose your OS
# 2. Download and install the binary with Homebrew
% brew tap grafana/grafana
% brew install grafana-agent
# 3. Set up the agent configurations
% mkdir /usr/local/etc/grafana-agent/
% hostname
Kens-MacBook-Pro.local
% vi /usr/local/etc/grafana-agent/config.yml
# Run the agent
% brew services start grafana-agent
# To remove it as a system service, run the following command
% brew services stop grafana-agent
# Note that when changing the configuration file for the Grafana Agent, you will need to restart the service.
% brew services restart grafana-agent

