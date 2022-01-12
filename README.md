# ansible-geolite-maxmind-agent-install
Ansible playbook to install the [Maxmind Geolite2 Update Program](https://dev.maxmind.com/geoip/updating-databases/?lang=en#using-geoip-update) and schedule a weekly update using cron.

## Requirements

Sign up for [Maxmind GeoLite2 account](https://www.maxmind.com/en/geolite2/signup?lang=en) and [create a license](https://www.maxmind.com/en/accounts/current/license-key?lang=en)

## Role Variables
Geo IP account Information (located in vars.yml file)

    geoip_account: <Account number> 
    geoip_license: <license key>

Proxy

     If server is behind a proxy set use_proxy to yes and fill in variables.

    use_proxy: no

    Only required if use_proxy set to yes.
    proxy_ip: x.x.x.x
    proxy_port: 3128