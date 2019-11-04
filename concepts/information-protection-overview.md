---
title: Microsoft 信息保护标记概述
description: Microsoft 信息保护标签可帮助组织基于 Office 365 安全性和合规性中心敏感度标签对数据进行分类、标记和保护。
author: tommoser
localization_priority: Normal
ms.prod: microsoft.informationprotection
ms.openlocfilehash: 60815acab92bc0776ff18269c654a37252ffc512
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934779"
---
# <a name="information-protection-overview"></a>信息保护概述

Microsoft 信息保护可帮助组织根据[敏感度](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels)对数据进行分类、标记和保护。 

组织使用标签来帮助：

* 了解正在处理的信息的重要性的用户。
* 在发现敏感信息所在的地方的合规管理员。 
* 基于更丰富的标签信息部署数据访问和数据丢失防护策略的安全管理员。

## <a name="why-integrate-microsoft-information-protection"></a>为什么要集成 Microsoft 信息保护？ 

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>与无处不在的用户和设备服务集成在一起使用的标签平台

拥有数十万个用户的多万个组织使用 Microsoft 信息保护对数据进行分类、添加标签和保护。  除了 Office 365 之外，各种数据丢失防护（DLP）服务、商业智能平台和软件即用服务（SaaS）解决方案都采用[Microsoft 信息保护](https://www.microsoft.com/en-us/security/technology/information-protection)标签，以提供更丰富的数据分类体验. 

### <a name="label-information-in-line-of-business-applications"></a>在业务线应用程序中添加标签信息

企业开发人员使用 Microsoft 信息保护在从业务线应用程序中导出时标记和保护敏感的客户信息，以确保客户信息的安全。 将应用程序连接到 Microsoft 信息保护生态系统使应用程序能够在自己的应用程序数据中应用、更新和删除[敏感度标签](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels)，而不会导致集成完整 SDK 的开销。

## <a name="what-can-i-do-with-microsoft-information-protection-label-apis-in-microsoft-graph"></a>在 Microsoft Graph 中，我可以使用 Microsoft 信息保护标签 Api 做什么？ 

### <a name="discover-labels-available-to-a-user-or-organization"></a>发现用户或组织可以使用的标签

使用 Microsoft Graph，可以访问用户或组织可用的[敏感度标签](/graph/api/informationprotectionlabel.md?view=graph-rest-beta)。 标签由应用程序和服务应用于静止数据或移动数据，可帮助用户和下游应用程序和服务了解正在处理的信息的敏感度。

### <a name="understand-how-to-apply-labels"></a>了解如何应用标签

通过提供有关现有和所需敏感度标签的信息，REST API 可智能地通知应用程序应采取的[操作](/graph/api/resources/informationProtectionActions.md?view=graph-rest-beta)才能正确应用标签。 这包括[元数据](/graph/api/resources/metadataaction.md?view=graph-rest-beta)应用程序、[水印](/graph/api/resources/addwatermarkaction.md?view=graph-rest-beta)生成、[保护](/graph/api/resources/protectByTemplateAction.md?view=graph-rest-beta)等操作。

### <a name="interpret-labels-applied-to-data"></a>解释应用于数据的标签

如果应用程序使用已应用了[敏感性标签元数据](/graph/api/resources/metadataaction.md?view=graph-rest-beta)的信息，则可以使用**extractLabel** API 将标签元数据解析为 Microsoft 信息保护[灵敏度标签](/graph/api/resources/informationprotectionlabel.md?view=graph-rest-beta)。 使用标签标识在处理或使用标记的数据时应由应用程序执行的操作。 

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [Microsoft Graph beta 中的 microsoft 信息保护 API](/graph/api/resources/information-protection-overview?view=graph-rest-beta)

## <a name="next-steps"></a>后续步骤

- 选择并尝试在[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中标记示例查询的信息保护。 选择左侧列中的“显示更多示例”****。 使用菜单打开 " **Microsoft 信息保护**"。
