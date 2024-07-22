# EMQX 5.5 中的不兼容变更

## v5.5.0

MQTT 数据桥接的管理方式进行了重构和拆分，以提供更灵活和高效的管理方式。
原本通过 `/bridges` API 进行管理的操作现在被拆分到了 `/connectors`, `/actions` 和 `/sources` 这三个 API 中。这样的拆分能够更细粒度地控制和管理 MQTT 数据桥接的各个部分，提高了系统的灵活性和可用性。
对于旧版本中的配置，用户需要按照 [与其他 MQTT 服务桥接](../data-integration/data-bridge-mqtt.md) 的指南重新配置进行手动迁移。这个迁移过程可能需要一些时间和精力，但是完成后用户可以享受到新版本优化带来的好处。