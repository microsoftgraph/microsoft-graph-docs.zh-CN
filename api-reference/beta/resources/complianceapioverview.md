---
title: 使用Microsoft Graph合规性和隐私 API
description: Microsoft Graph合规性和隐私 API 提供统一的界面和架构，以与 Microsoft 和生态系统合作伙伴在合规中心提供的解决方案集成。 这可以帮助客户简化其合规性和隐私操作，以便更好地管理和监视其数据、保护信息、最大程度地降低内部风险、执行法律和内部调查以及遵守法律或法规标准。
ms.localizationpriority: high
author: mahage-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: 3a038b2d481afa681f1003de0d1c46b5c4c8e5ea
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441424"
---
# <a name="use-the-microsoft-graph-compliance-and-privacy-apis"></a>使用Microsoft Graph合规性和隐私 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph合规性和隐私 API 提供统一的界面和架构，以与 Microsoft 和生态系统合作伙伴在合规中心提供的解决方案集成。 这可以帮助客户简化其合规性和隐私操作，以便更好地管理和监视其数据、保护信息、最大程度地降低内部风险、执行法律和内部调查以及遵守法律或法规标准。 有关详细信息，请参阅 [Microsoft 365 合规性文档](/microsoft-365/compliance)。

使用Microsoft Graph合规性和隐私 API 生成以下应用程序：

- 自动化电子数据展示中的常见任务
- 创建和管理使用者权限请求
- 在记录管理中自动执行任务

## <a name="ediscovery"></a>电子数据展示

Microsoft 365中的电子数据展示提供了端到端工作流，用于保留、收集、查看、分析和导出响应组织内部和外部调查的数据。详细了解 [Microsoft 365高级电子数据展示](/microsoft-365/compliance/overview-ediscovery-20)。

浏览[Microsoft 365电子数据展示 API](ediscovery-ediscoveryapioverview.md)。

## <a name="subject-rights-request"></a>使用者权限请求

Microsoft Priva 主体权利请求提供了强大的功能，可帮助你处理组织中来自寻求管理个人数据的人员的请求。 这些请求有时也称为数据主体请求 （DSR）、数据主体访问请求 （DSAR） 或使用者权限请求。 Microsoft Priva 使负责满足主体权利请求的人员能够轻松识别数据主体，并在 Exchange、SharePoint、OneDrive 和 Teams 中的组织数据中查找他们的个人信息。 了解有关 [Priva 主体权利请求](/microsoft-365/compliance/privacy-management-subject-rights-requests)的详细信息。

浏览[主体权利请求 API](subjectrightsrequest-subjectrightsrequestapioverview.md)。

## <a name="records-management-preview"></a>记录管理 (预览版)

Microsoft Purview 中的记录管理提供跨公司数据管理法规、法律和业务关键记录的功能。 它帮助组织管理数据的保留和删除，以满足其法律义务和合规性法规，并通过对不再需要保留的项目进行定期处置来提高效率。

更多相关详细信息，请参阅 [Microsoft Purview 记录管理](/microsoft-365/compliance/records-management)。

记录管理 API 在 OData 子名称空间 microsoft.graph.security 中定义。
浏览 [Microsoft Purview 记录管理 API](security-recordsManagement-overview.md)。

<!--
## Labels

??? Labels should be moved from security to here.  They are currently under a node called Information protection.
-->
