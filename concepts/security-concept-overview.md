# <a name="overview-of-security-in-microsoft-graph-preview"></a>Microsoft Graph 安全性概述（预览版） 

你可以使用 Microsoft Graph 连接 Intelligent Security Graph，以利用 Microsoft 和安全合作伙伴资源，并构建更好的威胁响应解决方案。 Microsoft Graph 还可以提供对由 Azure Active Directory (Azure AD) 中的 Identity Protection 服务检测到的用户和帐户风险的访问权限，使你能够将帐户风险数据集成到安全应用程序中。

## <a name="why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph"></a>为什么要使用安全 API 并连接 Microsoft Intelligent Security Graph？

Intelligent Security Graph 是一个用于对抗网络威胁的统一平台。 它为 Microsoft 产品和服务提供实时威胁保护，并支持集成了解决方案的生态系统。

[Microsoft Graph 中的安全性 API](https://aka.ms/graphsecuritydocs) 使你可以轻松与 Intelligent Security Graph 中的这些解决方案进行连接。 它使你可以更容易地实现并丰富这些解决方案的价值。

### <a name="unify-and-standardize-alert-management"></a>统一和标准化警报管理

使用通用警报架构可以更容易地跨安全性解决方案关联警报。 编写一次代码，即可集成来自任何 Microsoft Graph 已集成安全性解决方案的警报，并跨所有解决方案同步保持警报状态和分配。 你还可以通过 [Azure Monitor](https://docs.microsoft.com/zh-CN/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub) 将警报流式传输到安全性信息和事件管理 (SIEM) 解决方案，如 Splunk 和 IBM QRadar。

### <a name="federated-security-aggregation-service"></a>联合安全聚合服务

使用安全性 API 作为联合安全聚合服务，可向所有已启用的安全提供程序提交查询，并获得聚合响应。

### <a name="unlock-security-context-to-drive-investigation"></a>解锁安全性上下文以推动调查

深入到相关的安全相关库存（如用户、主机和应用），然后添加来自其他 Microsoft Graph 提供程序（Azure AD、Microsoft Intune、Office 365）的组织上下文，以将业务和安全性上下文结合在一起并改进威胁响应。

## <a name="why-use-azure-ad-to-protect-identities-in-your-organization"></a>为什么要使用 Azure AD 来保护组织中的身份信息？

大多数安全漏洞都会导致攻击者窃取用户的身份，攻击者利用第三方漏洞、密码喷洒攻击和复杂的网络钓鱼攻击，从而使攻击变得非常有效。 这就意味着，你需要保护所有用户帐户免受这些攻击，并主动防止泄露的身份信息被滥用。

Azure AD 使用自适应机器学习算法和启发式方法来检测异常情况，指示可能会遭到入侵的帐户。 使用此数据，Identity Protection 可使用基于风险的条件访问策略保护用户，并根据其检测结果生成报告和警报。

现在，Microsoft Graph 可轻松访问 Azure AD Premium P1 和 P2 客户，以查询 Identity Protection 所做的风险检测，并在 SIEM 系统和安全应用程序中使用这些事件。

## <a name="next-steps"></a>后续步骤

- [使用安全性 API](../api-reference/beta/resources/security-api-overview.md)
- [使用 Azure AD Identity Protection](../api-reference/beta/resources/identityprotection_root.md)

