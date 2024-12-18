---
title: "Portainer Agent"
---

Homepage: [https://www.portainer.io/](https://www.portainer.io/)

Portainer Agent is a companion service for Portainer that enables you to manage remote Docker hosts. The agent is designed to be lightweight and easy to deploy.

## Usage

Set `portainer_agent_enabled: true` in your `inventories/<your_inventory>/group_vars/nas.yml` file.

The Portainer Agent will be available on port 9001. You can add this endpoint to your Portainer installation by going to Endpoints > Add Endpoint > Agent and entering `ansible_nas_host_or_ip:9001`.

## Specific Configuration

1. In your Portainer installation, navigate to Endpoints > Add Endpoint
2. Select "Agent" as the endpoint type
3. Enter the name for your endpoint
4. In the "Environment URL" field, enter `ansible_nas_host_or_ip:9001`
5. Click "Add Endpoint"

The remote Docker host should now be available to manage through your Portainer installation.
