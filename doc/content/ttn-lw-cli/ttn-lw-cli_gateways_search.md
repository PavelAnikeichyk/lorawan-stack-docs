---
title: "ttn-lw-cli gateways search"
slug: ttn-lw-cli_gateways_search
---

## ttn-lw-cli gateways search

Search for gateways

```
ttn-lw-cli gateways search [flags]
```

### Options

```
      --administrative-contact                                        select the administrative_contact field and all allowed sub-fields
      --administrative-contact.ids.organization-ids                   select the administrative_contact.ids.organization_ids field and all allowed sub-fields
      --administrative-contact.ids.organization-ids.organization-id   select the administrative_contact.ids.organization_ids.organization_id field
      --administrative-contact.ids.user-ids                           select the administrative_contact.ids.user_ids field and all allowed sub-fields
      --administrative-contact.ids.user-ids.email                     select the administrative_contact.ids.user_ids.email field
      --administrative-contact.ids.user-ids.user-id                   select the administrative_contact.ids.user_ids.user_id field
      --all                                                           select all gateway fields
      --antennas                                                      select the antennas field
      --attributes                                                    select the attributes field
      --attributes-contain stringToString                             (key=value) (default [])
      --auto-update                                                   select the auto_update field
      --claim-authentication-code                                     select the claim_authentication_code field and all allowed sub-fields
      --claim-authentication-code.secret                              select the claim_authentication_code.secret field and all allowed sub-fields
      --claim-authentication-code.secret.key-id                       select the claim_authentication_code.secret.key_id field
      --claim-authentication-code.secret.value                        select the claim_authentication_code.secret.value field
      --claim-authentication-code.valid-from                          select the claim_authentication_code.valid_from field
      --claim-authentication-code.valid-to                            select the claim_authentication_code.valid_to field
      --contact-info                                                  select the contact_info field
      --deleted                                                       return recently deleted
      --deleted-at                                                    select the deleted_at field
      --description                                                   select the description field
      --description-contains string                                   
      --disable-packet-broker-forwarding                              select the disable_packet_broker_forwarding field
      --downlink-path-constraint                                      select the downlink_path_constraint field
      --enforce-duty-cycle                                            select the enforce_duty_cycle field
      --eui-contains string                                           
      --frequency-plan-id                                             select the frequency_plan_id field
      --frequency-plan-ids                                            select the frequency_plan_ids field
      --gateway-server-address                                        select the gateway_server_address field
  -h, --help                                                          help for search
      --id-contains string                                            
      --lbs-lns-secret                                                select the lbs_lns_secret field and all allowed sub-fields
      --lbs-lns-secret.key-id                                         select the lbs_lns_secret.key_id field
      --lbs-lns-secret.value                                          select the lbs_lns_secret.value field
      --limit uint32                                                  maximum number of results to get (default 50)
      --location-public                                               select the location_public field
      --lrfhss                                                        select the lrfhss field and all allowed sub-fields
      --lrfhss.supported                                              select the lrfhss.supported field
      --name                                                          select the name field
      --name-contains string                                          
      --order string                                                  order by this field
      --page uint32                                                   results page number (default 1)
      --require-authenticated-connection                              select the require_authenticated_connection field
      --schedule-anytime-delay                                        select the schedule_anytime_delay field
      --schedule-downlink-late                                        select the schedule_downlink_late field
      --status-public                                                 select the status_public field
      --target-cups-key                                               select the target_cups_key field and all allowed sub-fields
      --target-cups-key.key-id                                        select the target_cups_key.key_id field
      --target-cups-key.value                                         select the target_cups_key.value field
      --target-cups-uri                                               select the target_cups_uri field
      --technical-contact                                             select the technical_contact field and all allowed sub-fields
      --technical-contact.ids.organization-ids                        select the technical_contact.ids.organization_ids field and all allowed sub-fields
      --technical-contact.ids.organization-ids.organization-id        select the technical_contact.ids.organization_ids.organization_id field
      --technical-contact.ids.user-ids                                select the technical_contact.ids.user_ids field and all allowed sub-fields
      --technical-contact.ids.user-ids.email                          select the technical_contact.ids.user_ids.email field
      --technical-contact.ids.user-ids.user-id                        select the technical_contact.ids.user_ids.user_id field
      --update-channel                                                select the update_channel field
      --update-location-from-status                                   select the update_location_from_status field
      --version-ids                                                   select the version_ids field and all allowed sub-fields
      --version-ids.brand-id                                          select the version_ids.brand_id field
      --version-ids.firmware-version                                  select the version_ids.firmware_version field
      --version-ids.hardware-version                                  select the version_ids.hardware_version field
      --version-ids.model-id                                          select the version_ids.model_id field
```

### Options inherited from parent commands

```
      --allow-unknown-hosts                             Allow sending credentials to unknown hosts
      --application-server-enabled                      Application Server enabled (default true)
      --application-server-grpc-address string          Application Server address (default "localhost:8884")
      --ca string                                       CA certificate file
  -c, --config strings                                  Location of the config files (default [.ttn-lw-cli.yml,$HOME/.ttn-lw-cli.yml,$HOME/.config/.ttn-lw-cli.yml])
      --credentials-id string                           Credentials ID (if using multiple configurations)
      --device-claiming-server-grpc-address string      Device Claiming Server address (default "localhost:8884")
      --device-template-converter-grpc-address string   Device Template Converter address (default "localhost:8884")
      --dump-requests                                   When log level is set to debug, also dump request payload as JSON
      --experimental.features strings                   Experimental features to activate
      --gateway-server-enabled                          Gateway Server enabled (default true)
      --gateway-server-grpc-address string              Gateway Server address (default "localhost:8884")
      --identity-server-grpc-address string             Identity Server address (default "localhost:8884")
      --input-format string                             Input format (default "json")
      --insecure                                        Connect without TLS
      --join-server-enabled                             Join Server enabled (default true)
      --join-server-grpc-address string                 Join Server address (default "localhost:8884")
      --log.format string                               Log format to write (console, json) (default "console")
      --log.level string                                The minimum level log messages must have to be shown (default "info")
      --network-server-enabled                          Network Server enabled (default true)
      --network-server-grpc-address string              Network Server address (default "localhost:8884")
      --oauth-server-address string                     OAuth Server address (default "https://localhost/oauth")
      --output-format string                            Output format (default "json")
      --packet-broker-agent-grpc-address string         Packet Broker Agent address (default "localhost:8884")
      --qr-code-generator-grpc-address string           QR Code Generator address (default "localhost:8884")
      --retry-config.default-timeout duration           Default timeout between retry attempts (default 100ms)
      --retry-config.enable-metadata                    Use request response metadata to dynamically calculate timeout between retry attempts (default true)
      --retry-config.jitter float                       Fraction that creates a deviation of the timeout used between retry attempts
      --retry-config.max uint                           Maximum amount of times that a request can be reattempted
      --skip-version-check                              Do not perform version checks
```

### SEE ALSO

* [ttn-lw-cli gateways]({{< relref "ttn-lw-cli_gateways" >}})	 - Gateway commands
