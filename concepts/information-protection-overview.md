---
title: Microsoft 信息保护标签概述
description: Microsoft 信息保护标签可帮助组织根据安全与合规中心敏感度标签Office 365分类、标记和保护数据。
author: tommoser
ms.localizationpriority: medium
ms.prod: security
ms.openlocfilehash: 9731bd91f8e8eb42bfc7355a4eba69cc512db0f1
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220379"
---
# <a name="information-protection-overview"></a>信息保护概述

Microsoft 信息保护可帮助组织根据敏感度对数据进行分类、标记[和保护](/Office365/SecurityCompliance/sensitivity-labels)。 

组织使用标签帮助：

* 了解正在处理的信息重要性的用户。
* 合规性管理员，负责发现敏感信息的存储位置。 
* 安全管理员基于更丰富的标签信息部署数据访问和数据丢失防护策略。

## <a name="why-integrate-microsoft-information-protection"></a>为什么集成Microsoft 信息保护？ 

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>与无处不在的标签平台集成，为数百万用户和设备提供服务

拥有数千万用户的一百多万个组织Microsoft 信息保护分类、标记和保护数据。  除了 Microsoft 365，各种数据丢失防护 (DLP) 服务、商业智能 平台和软件即服务 (SaaS) 解决方案还支持 Microsoft 信息保护 标签，以提供更加丰富的数据分类[体验](https://www.microsoft.com/security/technology/information-protection)。 

### <a name="label-information-in-line-of-business-applications"></a>在业务线应用程序中标记信息

Enterprise开发人员Microsoft 信息保护在从业务线应用程序导出时标记和保护敏感的客户信息，以确保客户信息安全。 将应用程序连接到 Microsoft 信息保护 生态系统使应用程序能够在自己的应用程序数据中应用、更新和删除[](/Office365/SecurityCompliance/sensitivity-labels)敏感度标签，而无需集成完整 SDK 的开销。

## <a name="what-can-i-do-with-microsoft-information-protection-label-apis-in-microsoft-graph"></a>使用 Microsoft Microsoft 信息保护 中的标签 API 可以Graph？ 

### <a name="discover-labels-available-to-a-user-or-organization"></a>发现可供用户或组织使用的标签

使用 Microsoft Graph可以访问用户或组织可用的[](/graph/api/informationprotectionlabel?view=graph-rest-beta)敏感度标签。 标签由应用程序和服务应用于处于其余状态或动态的数据，帮助用户和下游应用程序和服务了解所处理信息的敏感性。

### <a name="understand-how-to-apply-labels"></a>了解如何应用标签

通过提供现有和所需敏感度标签的信息，REST API 可以智能地通知应用正确应用标签应采取的操作[](/graph/api/resources/informationprotectionaction?view=graph-rest-beta)。 这包括元数据应用程序 [、](/graph/api/resources/metadataaction?view=graph-rest-beta) 水 [印](/graph/api/resources/addwatermarkaction?view=graph-rest-beta) 生成 [、保护](/graph/api/resources/protectbytemplateaction?view=graph-rest-beta)等操作。

### <a name="interpret-labels-applied-to-data"></a>解释应用于数据的标签

使用已应用了敏感度标签 [](/graph/api/resources/metadataaction?view=graph-rest-beta)元数据的信息的应用程序可以使用 **extractLabel** API 将标签元数据解析为Microsoft 信息保护 [标签](/graph/api/resources/informationprotectionlabel.md?view=graph-rest-beta)。 使用标签可标识应用程序在处理或使用已标记数据时应该采取的操作。 

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [Microsoft 信息保护Microsoft Graph beta 中的 API](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta)

## <a name="next-steps"></a>后续步骤

- 在资源管理器 中选择并尝试信息保护标记Graph[查询](https://developer.microsoft.com/graph/graph-explorer)。 选择左侧列中的“显示更多示例”。 使用菜单打开 **"Microsoft 信息保护"。**
