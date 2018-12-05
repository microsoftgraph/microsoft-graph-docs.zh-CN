---
title: Microsoft Graph 安全 API 概述
description: 您可以使用 Microsoft Graph 安全 API 连接 Microsoft 安全产品、 服务和合作伙伴简化安全性操作以及提高威胁保护、 检测和响应能力。 Microsoft Graph 安全 API 为中间服务 （或代理），它提供单个的编程接口连接多个 Microsoft Graph 安全提供程序 (也称为安全提供程序或提供程序)。 对 Microsoft Graph 安全 API 请求对所有适用的安全提供程序联盟。 聚合结果并返回到请求应用程序中常见的架构，如下图中所示。 有关详细信息，请参阅 Microsoft Graph 安全 API 数据流。
ms.openlocfilehash: b5e1fb3d60cfc55cb940a217aaba872175887297
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091765"
---
# <a name="microsoft-graph-security-api-overview"></a>Microsoft Graph 安全 API 概述

您可以使用 Microsoft Graph 安全 API 连接 Microsoft 安全产品、 服务和合作伙伴简化安全性操作以及提高威胁保护、 检测和响应能力。 Microsoft Graph 安全 API 为中间服务 （或代理），它提供单个的编程接口连接多个[Microsoft Graph 安全提供程序](/graph/api/resources/securityvendorinformation?view=graph-rest-1.0)(也称为安全提供程序或提供程序)。 对 Microsoft Graph 安全 API 请求对所有适用的安全提供程序联盟。 聚合结果并返回到请求应用程序中常见的架构，如下图中所示。 有关详细信息，请参阅[Microsoft Graph 安全 API 数据流](security-dataflow.md)。

![security_overview_diagram_1.png](./images/security-overview-diagram-1.png)

有关授权的信息，请参阅[Authorization and Microsoft Graph 安全 API](security-authorization.md)。 有关权限的信息，包括委派和应用程序权限，请参阅[Permissions](permissions-reference.md#security-permissions)。

## <a name="why-use-the-microsoft-graph-security-api"></a>为什么使用 Microsoft Graph 安全 API？

[Microsoft Graph 安全 API](/graph/api/resources/security-api-overview?view=graph-rest-1.0)可以轻松地与其他 Microsoft 和 Microsoft 合作伙伴安全产品和服务。 它使你可以更容易地实现并丰富这些解决方案的价值。

### <a name="unify-and-standardize-alert-tracking"></a>统一和标准化警报跟踪

一次编写代码以跨所有解决方案集成从任何 Microsoft Graph 集成安全性解决方案和保留警报状态和分配同步的通知。 此外可以传输到安全信息和事件管理 (SIEM) 解决方案，如 Splunk 和 IBM QRadar，通过[Azure 监视器](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub)的通知。 有关安全 API 实体 SIEM 集成的详细信息，请参阅[SIEM 集成](security-siemintegration.md)。

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>关联安全警告，以提高威胁保护和响应

通知跨关联的安全解决方案更轻松地与警报的统一架构。 这不仅可以接收切实可行警报的信息，但允许安全分析师数据透视表和丰富使用资产和用户信息，启用更快地响应威胁和资产保护的通知。  

### <a name="update-alert-tags-status-and-assignments"></a>更新警报标签、 状态和分配

与其他上下文或威胁智能以告知响应和修正标记通知。 确保所有工作流的可见性捕获注释和通知的反馈。 将保留警报状态和分配同步，以便所有的集成的解决方案反映的当前状态。 使用 webhook 订阅来获取通知的更改。  

### <a name="unlock-security-context-to-drive-investigation"></a>解锁安全性上下文以推动调查

深入到相关的安全相关库存（如用户、主机和应用），然后添加来自其他 Microsoft Graph 提供程序（Azure AD、Microsoft Intune、Office 365）的组织上下文，以将业务和安全性上下文结合在一起并改进威胁响应。

### <a name="proactively-manage-security-risks-preview"></a>主动管理安全风险 （预览）

使用 Microsoft 安全分数 （预览） 提供可见的组织的安全需求并获取有关如何提高，建议项目改进的分数之后采用这些建议。 轻松随着时间的推移衡量进度并获取特定更改导致您分数改善见解。

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全 API 的好处

下表列出了不同的安全解决方案可以访问通过与 Microsoft Graph 安全 API 集成的好处。  

|**区域**     | **优点**|
|:---------------|:---------|
|**管理安全服务提供商 (MSSPs)**|<ul><li>简化了安全操作工具和服务的集成。</li> <li>减少了的部署和维护时间和工作。</li> <li>向 MSSP 客户提供更多价值的能力。</li></ul>|
|**SIEM 和 IT 风险管理解决方案**|<ul><li>Microsoft 安全解决方案和合作伙伴生态系统的平滑地集成。</li> <li>富通知元数据。</li> <li>更好的警报关联。</li></ul>|
|**应用程序** <br>（威胁智能、 移动、 云、 IOT、 欺诈检测、 标识和访问、 风险和合规性、 防火墙，等等）|<ul><li>跨越各种安全解决方案统一威胁管理、 预防和风险管理。</li> <li>通知、 库存、 配置，和通过 Microsoft Graph 公开的操作。</li> <li>与 Microsoft Graph 启用解决方案的即时集成。</li></ul>|

## <a name="api-reference"></a>API 参考
正在寻找此服务的 API 参考？

- [Microsoft Graph v1.0 中的安全性 API](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- [Microsoft Graph beta 中的安全 API](/graph/api/resources/security-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft Graph 安全 API](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- 希望成为安全提供程序？ 访问的[graphsecfeedback](mailto:graphsecfeedback@microsoft.com)。
