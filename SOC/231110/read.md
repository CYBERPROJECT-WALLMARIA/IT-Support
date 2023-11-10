502 Error

Issue Reason: Insufficient Disk Quota

{"service":{"node":{"roles":["background_tasks","ui"]}},"ecs":{"version":"8.6.1"},"@timestamp":"2023-11-10T03:53:06.163+00:00","message":"Failed to activate user profile: {\"error\":{\"root_cause\":[{\"type\":\"cluster_block_exception\",\"reason\":\"index [.security-profile-8] blocked by: [TOO_MANY_REQUESTS/12/disk usage exceeded flood-stage watermark, index has read-only-allow-delete block];\"}],\"type\":\"cluster_block_exception\",\"reason\":\"index [.security-profile-8] blocked by: [TOO_MANY_REQUESTS/12/disk usage exceeded flood-stage watermark, index has read-only-allow-delete block];\"},\"status\":429}.","log":{"level":"ERROR","logger":"plugins.security.user-profile"},"process":{"pid":7},"trace":{"id":"8c6f4c3446e46c864529078c9cda6a1f"},"transaction":{"id":"5c23c05ea9206e35"}}
