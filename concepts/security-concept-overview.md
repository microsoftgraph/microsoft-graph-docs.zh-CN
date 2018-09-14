# <a name="microsoft-graph-security-api-overview"></a>Microsoft Graph 安全性 API 概述

你可以使用 Microsoft Graph 安全性 API 连接 Microsoft 安全产品、服务和合作伙伴，以简化安全性操作并提高威胁防护、检测和响应能力。 Microsoft Graph 安全性 API 是一种提供单个程序设计界面以连接多个 [Microsoft Graph Security 提供程序](../api-reference/v1.0/resources/securityvendorinformation.md)（亦称为安全提供程序或提供程序）的中间服务（或代理）。 把对 Microsoft Graph 安全性 API 的请求聚合到所有适用的安全提供程序。 将结果汇集起来并用通用架构返回给请求应用程序，如下图所示。 有关详细信息，请参阅 [Microsoft Graph Security 数据流](security-dataflow.md)。

![security_overview_diagram_1.png](./images/security_overview_diagram_1.png)

有关授权的信息，请参阅 [授权和安全性 API](security-authorization.md)。 有关权限的信息，包括委派和应用程序权限，请参阅[权限](permissions_reference.md#security-permissions)。

## <a name="why-use-the-microsoft-graph-security-api"></a>为何使用 Microsoft Graph 安全性 API？

 [Microsoft Graph 安全性 API](../api-reference/v1.0/resources/security-api-overview.md) 可以轻松地与其他 Microsoft 和 Microsoft 合作伙伴的安全产品和服务连接。 它使你可以更容易地实现并丰富这些解决方案的价值。

### <a name="unify-and-standardize-alert-tracking"></a>统一和标准化警报跟踪

编写一次代码，即可集成来自任何 Microsoft Graph 集成安全性解决方案的警报，并横跨所有解决方案同步保持警报状态和工作分配。 你还可以通过 [Azure Monitor](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub) 将警报流式传输到安全性信息和事件管理 (SIEM) 解决方案，如 Splunk 和 IBM QRadar。 有关 SIEM 与安全性 API 实体集成的详细信息，请参阅 [与 SIEM 集成](security_siemintegration.md)。

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>关联安全警报，以提高威胁防护和响应能力

使用统一的警报架构可以更容易地跨安全解决方案把警报关联起来。 这不仅使你可以收到可操作警报信息，还使安全分析师可以使用资产和用户信息透视并丰富警报内容，从而对威胁和资产保护更快作出响应。  

### <a name="update-alert-tags-status-and-assignments"></a>更新警报标签、状态和工作分配

用其他上下文或威胁智能给警报做标记以告知响应和修正。 确保捕获的有关警报的注释和反馈对所有工作流都具有可见性。 保持警报状态和工作分配同步，以便所有的集成解决方案都反映当前的状态。 使用 Webhook 订阅来获取更改通知。  

### <a name="unlock-security-context-to-drive-investigation"></a>解锁安全性上下文以推动调查

深入到相关的安全相关库存（如用户、主机和应用），然后添加来自其他 Microsoft Graph 提供程序（Azure AD、Microsoft Intune、Office 365）的组织上下文，以将业务和安全性上下文结合在一起并改进威胁响应。

### <a name="proactively-manage-security-risks-preview"></a>主动管理安全风险 （预览）

使用 Microsoft 安全功能分数（预览）对组织的安全需求提供可见性并获取如何加以改善的建议，并在采用这些建议后突出显示改进的分数。 能轻松衡量进度随时间的变化并获取特定更改可导致分数提高的见解。

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全性 API 的好处

下表列出了不同的安全解决方案可以通过与 Microsoft Graph 安全性 API 集成来访问的优势。  

|**区域**     | **优势**|
|:---------------|:---------|
|**托管的安全服务提供商 (MSSPs)**|<ul><li>简化了安全操作工具和服务的集成。</li> <li>减少了部署和维护的时间和精力。</li> <li>有能力给 MSSP 客户提供更多价值。</li></ul>|
|**SIEM 和 IT 风险管理解决方案**|<ul><li>可与 Microsoft 安全解决方案和生态系统合作伙伴顺利整合。</li> <li>丰富的警报元数据。</li> <li>更好的警报关联性。</li></ul>|
|**应用程序** <br>（威胁智能、手机、云、物联网、欺诈检测、标识和访问、风险和合规性、防火墙等等）|<ul><li>跨各种安全解决方案的统一威胁管理、预防和风险管理。</li> <li>警报、库存、配置和通过 Microsoft Graph 公开的操作。</li> <li>可与 Microsoft Graph 启用解决方案即时整合。</li></ul>|

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft Graph 安全性 API](../api-reference/v1.0/resources/security-api-overview.md)
- 对成为安全提供程商感兴趣？ 访问 [graphsecfeedback](mailto:graphsecfeedback@microsoft.com)。
