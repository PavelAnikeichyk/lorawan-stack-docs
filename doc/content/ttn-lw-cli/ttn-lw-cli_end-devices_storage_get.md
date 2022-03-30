---
title: "ttn-lw-cli end-devices storage get"
slug: ttn-lw-cli_end-devices_storage_get
---

## ttn-lw-cli end-devices storage get

Retrieve stored upstream messages

```
ttn-lw-cli end-devices storage get [application-id] [device-id] [flags]
```

### Options

```
      --after string                                                                     query upstream messages after specified timestamp (format: '2006-01-02 15:04:05')
      --after-utc string                                                                 query upstream messages after specified timestamp (format: '2006-01-02 15:04:05') (UTC)
      --application-id string                                                            
      --before string                                                                    query upstream messages before specified timestamp (format: '2006-01-02 15:04:05')
      --before-utc string                                                                query upstream messages before specified timestamp (format: '2006-01-02 15:04:05') (UTC)
      --correlation-ids                                                                  select the correlation_ids field
      --dev-eui string                                                                   (hex)
      --device-id string                                                                 
      --end-device-ids                                                                   select the end_device_ids field and all allowed sub-fields
      --end-device-ids.application-ids                                                   select the end_device_ids.application_ids field and all allowed sub-fields
      --end-device-ids.application-ids.application-id                                    select the end_device_ids.application_ids.application_id field
      --end-device-ids.dev-addr                                                          select the end_device_ids.dev_addr field
      --end-device-ids.dev-eui                                                           select the end_device_ids.dev_eui field
      --end-device-ids.device-id                                                         select the end_device_ids.device_id field
      --end-device-ids.join-eui                                                          select the end_device_ids.join_eui field
      --f-port uint32                                                                    query upstream messages with specific FPort
  -h, --help                                                                             help for get
      --join-eui string                                                                  (hex)
      --last duration                                                                    query upstream messages in the last hours or minutes
      --limit uint32                                                                     limit number of upstream messages to fetch
      --order string                                                                     order results (received_at|-received_at)
      --received-at                                                                      select the received_at field
      --simulated                                                                        select the simulated field
      --stream-output                                                                    print output as JSON stream
      --type string                                                                      message type (allowed values: , downlink_ack, downlink_failed, downlink_nack, downlink_queue_invalidated, downlink_queued, downlink_sent, join_accept, location_solved, service_data, uplink_message)
      --up.downlink-ack                                                                  select the up.downlink_ack field and all allowed sub-fields
      --up.downlink-ack.class-b-c                                                        select the up.downlink_ack.class_b_c field and all allowed sub-fields
      --up.downlink-ack.class-b-c.absolute-time                                          select the up.downlink_ack.class_b_c.absolute_time field
      --up.downlink-ack.class-b-c.gateways                                               select the up.downlink_ack.class_b_c.gateways field
      --up.downlink-ack.confirmed                                                        select the up.downlink_ack.confirmed field
      --up.downlink-ack.correlation-ids                                                  select the up.downlink_ack.correlation_ids field
      --up.downlink-ack.decoded-payload                                                  select the up.downlink_ack.decoded_payload field and all allowed sub-fields
      --up.downlink-ack.decoded-payload-warnings                                         select the up.downlink_ack.decoded_payload_warnings field
      --up.downlink-ack.f-cnt                                                            select the up.downlink_ack.f_cnt field
      --up.downlink-ack.f-port                                                           select the up.downlink_ack.f_port field
      --up.downlink-ack.frm-payload                                                      select the up.downlink_ack.frm_payload field
      --up.downlink-ack.priority                                                         select the up.downlink_ack.priority field
      --up.downlink-ack.session-key-id                                                   select the up.downlink_ack.session_key_id field
      --up.downlink-failed                                                               select the up.downlink_failed field and all allowed sub-fields
      --up.downlink-failed.downlink                                                      select the up.downlink_failed.downlink field and all allowed sub-fields
      --up.downlink-failed.downlink.class-b-c                                            select the up.downlink_failed.downlink.class_b_c field and all allowed sub-fields
      --up.downlink-failed.downlink.class-b-c.absolute-time                              select the up.downlink_failed.downlink.class_b_c.absolute_time field
      --up.downlink-failed.downlink.class-b-c.gateways                                   select the up.downlink_failed.downlink.class_b_c.gateways field
      --up.downlink-failed.downlink.confirmed                                            select the up.downlink_failed.downlink.confirmed field
      --up.downlink-failed.downlink.correlation-ids                                      select the up.downlink_failed.downlink.correlation_ids field
      --up.downlink-failed.downlink.decoded-payload                                      select the up.downlink_failed.downlink.decoded_payload field and all allowed sub-fields
      --up.downlink-failed.downlink.decoded-payload-warnings                             select the up.downlink_failed.downlink.decoded_payload_warnings field
      --up.downlink-failed.downlink.f-cnt                                                select the up.downlink_failed.downlink.f_cnt field
      --up.downlink-failed.downlink.f-port                                               select the up.downlink_failed.downlink.f_port field
      --up.downlink-failed.downlink.frm-payload                                          select the up.downlink_failed.downlink.frm_payload field
      --up.downlink-failed.downlink.priority                                             select the up.downlink_failed.downlink.priority field
      --up.downlink-failed.downlink.session-key-id                                       select the up.downlink_failed.downlink.session_key_id field
      --up.downlink-failed.error                                                         select the up.downlink_failed.error field and all allowed sub-fields
      --up.downlink-nack                                                                 select the up.downlink_nack field and all allowed sub-fields
      --up.downlink-nack.class-b-c                                                       select the up.downlink_nack.class_b_c field and all allowed sub-fields
      --up.downlink-nack.class-b-c.absolute-time                                         select the up.downlink_nack.class_b_c.absolute_time field
      --up.downlink-nack.class-b-c.gateways                                              select the up.downlink_nack.class_b_c.gateways field
      --up.downlink-nack.confirmed                                                       select the up.downlink_nack.confirmed field
      --up.downlink-nack.correlation-ids                                                 select the up.downlink_nack.correlation_ids field
      --up.downlink-nack.decoded-payload                                                 select the up.downlink_nack.decoded_payload field and all allowed sub-fields
      --up.downlink-nack.decoded-payload-warnings                                        select the up.downlink_nack.decoded_payload_warnings field
      --up.downlink-nack.f-cnt                                                           select the up.downlink_nack.f_cnt field
      --up.downlink-nack.f-port                                                          select the up.downlink_nack.f_port field
      --up.downlink-nack.frm-payload                                                     select the up.downlink_nack.frm_payload field
      --up.downlink-nack.priority                                                        select the up.downlink_nack.priority field
      --up.downlink-nack.session-key-id                                                  select the up.downlink_nack.session_key_id field
      --up.downlink-queue-invalidated                                                    select the up.downlink_queue_invalidated field and all allowed sub-fields
      --up.downlink-queue-invalidated.downlinks                                          select the up.downlink_queue_invalidated.downlinks field
      --up.downlink-queue-invalidated.last-f-cnt-down                                    select the up.downlink_queue_invalidated.last_f_cnt_down field
      --up.downlink-queue-invalidated.session-key-id                                     select the up.downlink_queue_invalidated.session_key_id field
      --up.downlink-queued                                                               select the up.downlink_queued field and all allowed sub-fields
      --up.downlink-queued.class-b-c                                                     select the up.downlink_queued.class_b_c field and all allowed sub-fields
      --up.downlink-queued.class-b-c.absolute-time                                       select the up.downlink_queued.class_b_c.absolute_time field
      --up.downlink-queued.class-b-c.gateways                                            select the up.downlink_queued.class_b_c.gateways field
      --up.downlink-queued.confirmed                                                     select the up.downlink_queued.confirmed field
      --up.downlink-queued.correlation-ids                                               select the up.downlink_queued.correlation_ids field
      --up.downlink-queued.decoded-payload                                               select the up.downlink_queued.decoded_payload field and all allowed sub-fields
      --up.downlink-queued.decoded-payload-warnings                                      select the up.downlink_queued.decoded_payload_warnings field
      --up.downlink-queued.f-cnt                                                         select the up.downlink_queued.f_cnt field
      --up.downlink-queued.f-port                                                        select the up.downlink_queued.f_port field
      --up.downlink-queued.frm-payload                                                   select the up.downlink_queued.frm_payload field
      --up.downlink-queued.priority                                                      select the up.downlink_queued.priority field
      --up.downlink-queued.session-key-id                                                select the up.downlink_queued.session_key_id field
      --up.downlink-sent                                                                 select the up.downlink_sent field and all allowed sub-fields
      --up.downlink-sent.class-b-c                                                       select the up.downlink_sent.class_b_c field and all allowed sub-fields
      --up.downlink-sent.class-b-c.absolute-time                                         select the up.downlink_sent.class_b_c.absolute_time field
      --up.downlink-sent.class-b-c.gateways                                              select the up.downlink_sent.class_b_c.gateways field
      --up.downlink-sent.confirmed                                                       select the up.downlink_sent.confirmed field
      --up.downlink-sent.correlation-ids                                                 select the up.downlink_sent.correlation_ids field
      --up.downlink-sent.decoded-payload                                                 select the up.downlink_sent.decoded_payload field and all allowed sub-fields
      --up.downlink-sent.decoded-payload-warnings                                        select the up.downlink_sent.decoded_payload_warnings field
      --up.downlink-sent.f-cnt                                                           select the up.downlink_sent.f_cnt field
      --up.downlink-sent.f-port                                                          select the up.downlink_sent.f_port field
      --up.downlink-sent.frm-payload                                                     select the up.downlink_sent.frm_payload field
      --up.downlink-sent.priority                                                        select the up.downlink_sent.priority field
      --up.downlink-sent.session-key-id                                                  select the up.downlink_sent.session_key_id field
      --up.join-accept                                                                   select the up.join_accept field and all allowed sub-fields
      --up.join-accept.app-s-key                                                         select the up.join_accept.app_s_key field and all allowed sub-fields
      --up.join-accept.app-s-key.encrypted-key                                           select the up.join_accept.app_s_key.encrypted_key field
      --up.join-accept.app-s-key.kek-label                                               select the up.join_accept.app_s_key.kek_label field
      --up.join-accept.app-s-key.key                                                     select the up.join_accept.app_s_key.key field
      --up.join-accept.invalidated-downlinks                                             select the up.join_accept.invalidated_downlinks field
      --up.join-accept.pending-session                                                   select the up.join_accept.pending_session field
      --up.join-accept.received-at                                                       select the up.join_accept.received_at field
      --up.join-accept.session-key-id                                                    select the up.join_accept.session_key_id field
      --up.location-solved                                                               select the up.location_solved field and all allowed sub-fields
      --up.location-solved.attributes                                                    select the up.location_solved.attributes field
      --up.location-solved.location                                                      select the up.location_solved.location field and all allowed sub-fields
      --up.location-solved.location.accuracy                                             select the up.location_solved.location.accuracy field
      --up.location-solved.location.altitude                                             select the up.location_solved.location.altitude field
      --up.location-solved.location.latitude                                             select the up.location_solved.location.latitude field
      --up.location-solved.location.longitude                                            select the up.location_solved.location.longitude field
      --up.location-solved.location.source                                               select the up.location_solved.location.source field
      --up.location-solved.service                                                       select the up.location_solved.service field
      --up.service-data                                                                  select the up.service_data field and all allowed sub-fields
      --up.service-data.data                                                             select the up.service_data.data field and all allowed sub-fields
      --up.service-data.service                                                          select the up.service_data.service field
      --up.uplink-message                                                                select the up.uplink_message field and all allowed sub-fields
      --up.uplink-message.app-s-key                                                      select the up.uplink_message.app_s_key field and all allowed sub-fields
      --up.uplink-message.app-s-key.encrypted-key                                        select the up.uplink_message.app_s_key.encrypted_key field
      --up.uplink-message.app-s-key.kek-label                                            select the up.uplink_message.app_s_key.kek_label field
      --up.uplink-message.app-s-key.key                                                  select the up.uplink_message.app_s_key.key field
      --up.uplink-message.confirmed                                                      select the up.uplink_message.confirmed field
      --up.uplink-message.consumed-airtime                                               select the up.uplink_message.consumed_airtime field
      --up.uplink-message.decoded-payload                                                select the up.uplink_message.decoded_payload field and all allowed sub-fields
      --up.uplink-message.decoded-payload-warnings                                       select the up.uplink_message.decoded_payload_warnings field
      --up.uplink-message.f-cnt                                                          select the up.uplink_message.f_cnt field
      --up.uplink-message.f-port                                                         select the up.uplink_message.f_port field
      --up.uplink-message.frm-payload                                                    select the up.uplink_message.frm_payload field
      --up.uplink-message.last-a-f-cnt-down                                              select the up.uplink_message.last_a_f_cnt_down field
      --up.uplink-message.locations                                                      select the up.uplink_message.locations field
      --up.uplink-message.network-ids                                                    select the up.uplink_message.network_ids field and all allowed sub-fields
      --up.uplink-message.network-ids.cluster-id                                         select the up.uplink_message.network_ids.cluster_id field
      --up.uplink-message.network-ids.net-id                                             select the up.uplink_message.network_ids.net_id field
      --up.uplink-message.network-ids.tenant-id                                          select the up.uplink_message.network_ids.tenant_id field
      --up.uplink-message.received-at                                                    select the up.uplink_message.received_at field
      --up.uplink-message.rx-metadata                                                    select the up.uplink_message.rx_metadata field
      --up.uplink-message.session-key-id                                                 select the up.uplink_message.session_key_id field
      --up.uplink-message.settings                                                       select the up.uplink_message.settings field and all allowed sub-fields
      --up.uplink-message.settings.coding-rate                                           select the up.uplink_message.settings.coding_rate field
      --up.uplink-message.settings.concentrator-timestamp                                select the up.uplink_message.settings.concentrator_timestamp field
      --up.uplink-message.settings.data-rate                                             select the up.uplink_message.settings.data_rate field and all allowed sub-fields
      --up.uplink-message.settings.data-rate.modulation.fsk                              select the up.uplink_message.settings.data_rate.modulation.fsk field and all allowed sub-fields
      --up.uplink-message.settings.data-rate.modulation.fsk.bit-rate                     select the up.uplink_message.settings.data_rate.modulation.fsk.bit_rate field
      --up.uplink-message.settings.data-rate.modulation.lora                             select the up.uplink_message.settings.data_rate.modulation.lora field and all allowed sub-fields
      --up.uplink-message.settings.data-rate.modulation.lora.bandwidth                   select the up.uplink_message.settings.data_rate.modulation.lora.bandwidth field
      --up.uplink-message.settings.data-rate.modulation.lora.spreading-factor            select the up.uplink_message.settings.data_rate.modulation.lora.spreading_factor field
      --up.uplink-message.settings.data-rate.modulation.lrfhss                           select the up.uplink_message.settings.data_rate.modulation.lrfhss field and all allowed sub-fields
      --up.uplink-message.settings.data-rate.modulation.lrfhss.coding-rate               select the up.uplink_message.settings.data_rate.modulation.lrfhss.coding_rate field
      --up.uplink-message.settings.data-rate.modulation.lrfhss.modulation-type           select the up.uplink_message.settings.data_rate.modulation.lrfhss.modulation_type field
      --up.uplink-message.settings.data-rate.modulation.lrfhss.operating-channel-width   select the up.uplink_message.settings.data_rate.modulation.lrfhss.operating_channel_width field
      --up.uplink-message.settings.downlink                                              select the up.uplink_message.settings.downlink field and all allowed sub-fields
      --up.uplink-message.settings.downlink.antenna-index                                select the up.uplink_message.settings.downlink.antenna_index field
      --up.uplink-message.settings.downlink.invert-polarization                          select the up.uplink_message.settings.downlink.invert_polarization field
      --up.uplink-message.settings.downlink.tx-power                                     select the up.uplink_message.settings.downlink.tx_power field
      --up.uplink-message.settings.enable-crc                                            select the up.uplink_message.settings.enable_crc field
      --up.uplink-message.settings.frequency                                             select the up.uplink_message.settings.frequency field
      --up.uplink-message.settings.time                                                  select the up.uplink_message.settings.time field
      --up.uplink-message.settings.timestamp                                             select the up.uplink_message.settings.timestamp field
      --up.uplink-message.version-ids                                                    select the up.uplink_message.version_ids field and all allowed sub-fields
      --up.uplink-message.version-ids.band-id                                            select the up.uplink_message.version_ids.band_id field
      --up.uplink-message.version-ids.brand-id                                           select the up.uplink_message.version_ids.brand_id field
      --up.uplink-message.version-ids.firmware-version                                   select the up.uplink_message.version_ids.firmware_version field
      --up.uplink-message.version-ids.hardware-version                                   select the up.uplink_message.version_ids.hardware_version field
      --up.uplink-message.version-ids.model-id                                           select the up.uplink_message.version_ids.model_id field
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

* [ttn-lw-cli end-devices storage]({{< relref "ttn-lw-cli_end-devices_storage" >}})	 - Storage Integration
