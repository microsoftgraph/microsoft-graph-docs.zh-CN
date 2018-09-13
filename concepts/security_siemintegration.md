# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>将 Microsoft Graph 安全性 API 警报与 SIEM 集成

Microsoft Graph 安全性 API 通过单个 REST 端点，从所有 Microsoft 安全产品（统称 Microsoft Graph 安全提供程序）启用管理安全警报。某些组织可能已将 Azure 特定日志数据通过 Azure Monitor 引入 SIEM 解决方案。为了简化集成，通过 Microsoft Graph 安全性 API 实现的安全警报也可以通过 Azure Monitor 由客户对其订阅进行设置。如果组织已使用 SIEM 解决方案配置了 Azure Monitor 集成，那么除了通过 Azure Monitor 提供的现有数据外，您现在还可以轻松地流式传输组织的安全警报。

Azure Monitor 支持连接到多个 SIEM 产品的连接器。 有关支持的 SIEM 产品列表的信息，请参阅[发送监控数据到事件中心](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub)。 Microsoft Graph 安全性 API 集成目前可用于 [Splunk](https://splunkbase.splunk.com/) 和 [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem)。

有关 Microsoft Graph 安全性 API 集成特定 SIEM 解决方案的信息，请参阅：

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
