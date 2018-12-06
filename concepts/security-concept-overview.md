---
title: Microsoft Graph 安全性 API 概述
description: Microsoft Graph 安全性 API 可用于连接 Microsoft 安全产品、服务和合作伙伴，以简化安全操作并改进威胁防护、检测和响应功能。 作为中介服务（或代理），Microsoft Graph 安全性 API 提供了一个编程接口，用于连接多个 Microsoft Graph 安全提供程序（亦称为“安全提供程序”或“提供程序”）。 向 Microsoft Graph 安全性 API 发出的请求被联合到所有适用的安全提供程序。 结果以通用架构的形式聚合并返回到发出请求的应用，如下图所示。 有关详细信息，请参阅“Microsoft Graph 安全性 API 数据流”。
ms.openlocfilehash: b5e1fb3d60cfc55cb940a217aaba872175887297
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091765"
---
# <a name="microsoft-graph-security-api-overview"></a>Microsoft Graph 安全性 API 概述

Microsoft Graph 安全性 API 可用于连接 Microsoft 安全产品、服务和合作伙伴，以简化安全操作并改进威胁防护、检测和响应功能。 作为中介服务（或代理），Microsoft Graph 安全性 API 提供了一个编程接口，用于连接多个 [Microsoft Graph 安全提供程序](/graph/api/resources/securityvendorinformation?view=graph-rest-1.0)（亦称为“安全提供程序”或“提供程序”）。 向 Microsoft Graph 安全性 API 发出的请求被联合到所有适用的安全提供程序。 结果以通用架构的形式聚合并返回到发出请求的应用，如下图所示。 有关详细信息，请参阅 [Microsoft Graph 安全性 API 数据流](security-dataflow.md)。

![security_overview_diagram_1.png](./images/security-overview-diagram-1.png)

若要了解授权，请参阅[授权和 Microsoft Graph 安全性 API](security-authorization.md)。 若要了解委托的权限和应用权限等权限，请参阅[权限](permissions-reference.md#security-permissions)。

## <a name="why-use-the-microsoft-graph-security-api"></a>为什么要使用 Microsoft Graph 安全性 API？

使用 [Microsoft Graph 安全性 API](/graph/api/resources/security-api-overview?view=graph-rest-1.0)，可以轻松连接各个 Microsoft 和 Microsoft 合作伙伴安全产品和服务。 借助它，可以更容易地实现并丰富这些解决方案的价值。

### <a name="unify-and-standardize-alert-tracking"></a>统一和标准化警报跟踪

编写一次代码，即可集成来自任何已集成 Microsoft Graph 的安全解决方案的警报，并跨所有解决方案同步警报状态和分配。 还可以通过 [Azure Monitor](https://docs.microsoft.com/zh-CN/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub) 将警报流式处理到安全信息和事件管理 (SIEM) 解决方案（如 Splunk 和 IBM QRadar）。 若要详细了解 SIEM 与安全性 API 实体的集成，请参阅[与 SIEM 集成](security-siemintegration.md)。

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>关联安全警报以改进威胁防护和响应

使用统一警报架构，可以更轻松地跨安全解决方案关联警报。 这样一来，不仅能够接收可操作警报信息，还便于安全分析员使用资产和用户信息来透视和丰富警报，从而更快地响应威胁防护和资产保护。  

### <a name="update-alert-tags-status-and-assignments"></a>更新警报标记、状态和分配

标记使用其他上下文或威胁情报发出警报，通知响应和修复。 确保捕获有关警报的评论和反馈，实现所有工作流程的可见性。 保持警报状态和分配同步，使所有集成解决方案都能反映当前状态。 使用 Webhook 订阅获取变更通知。  

### <a name="unlock-security-context-to-drive-investigation"></a>解锁安全性上下文以推动调查

深入到相关的安全相关库存（如用户、主机和应用），然后添加来自其他 Microsoft Graph 提供程序（Azure AD、Microsoft Intune、Office 365）的组织上下文，以将业务和安全性上下文结合在一起并改进威胁响应。

### <a name="proactively-manage-security-risks-preview"></a>主动管理安全风险（预览版）

使用 Microsoft 安全功能分数（预览版）了解组织的安全需求，获取改进方法建议，并预测在采纳这些建议后的改进分数。 可以轻松度量一段时间内的进度，并获取有助于提高分数的具体变更的相关见解。

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全性 API 的优势

下表列出了各种安全解决方案与 Microsoft Graph 安全性 API 集成后获得的优势。  

|**区域**     | **优势**|
|:---------------|:---------|
|**托管安全服务提供程序 (MSSP)**|<ul><li>简化了与安全操作工具和服务集成的过程。</li> <li>缩减了部署和维护时间及工作量。</li> <li>能够为 MSSP 客户增值。</li></ul>|
|**SIEM 和 IT 风险管理解决方案**|<ul><li>与 Microsoft 安全解决方案和生态系统合作伙伴顺畅集成。</li> <li>丰富的警报元数据。</li> <li>提升了警报关联性。</li></ul>|
|**应用** <br>（威胁智能、移动、云、IOT、欺诈检测、标识和访问、风险和合规性、防火墙等）|<ul><li>跨各种安全解决方案统一了威胁管理、防护和风险管理。</li> <li>通过 Microsoft Graph 公开了警报、清单、配置和操作。</li> <li>与已启用 Microsoft Graph 的解决方案即时集成。</li></ul>|

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的安全性 API](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- [Microsoft Graph beta 中的安全性 API](/graph/api/resources/security-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft Graph 安全性 API](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- 想要成为安全提供程序？ 请联系 [graphsecfeedback](mailto:graphsecfeedback@microsoft.com)。
