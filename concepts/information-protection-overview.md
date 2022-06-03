---
title: Microsoft Purview 信息保护标签概述
description: Microsoft Purview 信息保护标签可帮助组织基于 Office 365 安全与合规中心敏感度标签对数据进行分类、标记和保护。
author: tommoser
ms.localizationpriority: medium
ms.prod: security
ms.openlocfilehash: e2f93def1a27e3a19866319650122ba6d4fca09b
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884230"
---
# <a name="information-protection-overview"></a>信息保护概述

Microsoft Purview 信息保护可帮助组织基于 [敏感度](/Office365/SecurityCompliance/sensitivity-labels)对数据进行分类、标记和保护。 

组织使用标签来帮助：

* 用户了解正在处理的信息的重要性。
* 发现敏感信息所在位置的合规性管理员。 
* 基于更丰富的标签信息部署数据访问和数据丢失防护策略时的安全管理员。

## <a name="why-integrate-microsoft-purview-information-protection"></a>为什么要集成 Microsoft Purview 信息保护？ 

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>与无处不在的标签平台集成，为数百万用户和设备提供服务

拥有数千万用户的 100 多万个组织使用 Microsoft Purview 信息保护对数据进行分类、标记和保护。  除了 Microsoft 365 之外，各种数据丢失防护 (DLP) 服务、商业智能平台和软件即服务 (SaaS) 解决方案都 [采用了 Microsoft Purview 信息保护](https://www.microsoft.com/security/technology/information-protection) 标签，以提供更丰富的数据分类体验。 

### <a name="label-information-in-line-of-business-applications"></a>业务线应用程序中的标签信息

企业开发人员使用 Microsoft Purview 信息保护来标记和保护有关从业务线应用程序导出的敏感客户信息，以确保客户信息的安全。 将应用程序连接到 Microsoft Purview 信息保护生态系统使应用程序能够在自己的应用程序数据中应用、更新和删除 [敏感度标签](/Office365/SecurityCompliance/sensitivity-labels) ，而无需集成完整 SDK 的开销。

## <a name="what-can-i-do-with-microsoft-purview-information-protection-label-apis-in-microsoft-graph"></a>如何在 Microsoft Graph 中使用 Microsoft Purview 信息保护标签 API？ 

### <a name="discover-labels-available-to-a-user-or-organization"></a>发现用户或组织可用的标签

借助 Microsoft Graph，可以访问用户或组织可用 [的敏感度标签](/graph/api/resources/informationprotectionlabel) 。 应用程序和服务将标签应用于静态或动态数据，帮助用户和下游应用程序和服务了解所处理信息的敏感度。

### <a name="understand-how-to-apply-labels"></a>了解如何应用标签

通过提供有关现有和所需敏感度标签的信息，REST API 可以智能地告知应用程序正确应用标签时应采取的 [操作](/graph/api/resources/informationprotectionaction) 。 这包括 [元数据](/graph/api/resources/metadataaction) 应用程序、 [水印](/graph/api/resources/addwatermarkaction) 生成、 [保护](/graph/api/resources/protectbytemplateaction)等操作。

### <a name="interpret-labels-applied-to-data"></a>解释应用于数据的标签

使用已应用 [敏感度标签元数据](/graph/api/resources/metadataaction) 的信息的应用程序可以使用 **extractLabel** API 将标签元数据解析为 Microsoft Purview 信息保护 [敏感度标签](/graph/api/resources/informationprotectionlabel)。 使用标签标识应用程序在处理或使用标记数据时应执行的操作。 

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [Microsoft Graph beta 中的 Microsoft Purview 信息保护 API](/graph/api/resources/informationprotectionlabel)

## <a name="next-steps"></a>后续步骤

- 在 [图形资源管理器](https://developer.microsoft.com/graph/graph-explorer)中选择并尝试信息保护标记示例查询。 选择左侧列中的“显示更多示例”。 使用菜单打开 **Microsoft Purview 信息保护**。
