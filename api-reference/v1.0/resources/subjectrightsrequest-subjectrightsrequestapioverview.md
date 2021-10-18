---
title: 使用 Microsoft Graph权限请求 API
description: 应用程序Microsoft 365权限请求 API 为组织提供了自动执行重复任务并与现有主体权限请求工具集成的功能，以构建可重复的工作流，帮助满足行业法规。
ms.localizationpriority: medium
author: skadam-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: 0f31c5358142e5a88ee8474bc9cb681eebcb529d
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450129"
---
# <a name="use-the-microsoft-graph-subject-rights-request-api"></a>使用 Microsoft Graph权限请求 API

根据全球的某些隐私法规，个人可以请求查看或管理公司收集的有关自己的个人数据。 这些请求在隐私管理解决方案中称为Microsoft 365权限请求;它们有时也称为数据主体请求 (DSR) 或数据主体访问请求 (DSAR) 。 Microsoft 365隐私管理使负责履行主体权利请求的人员能够轻松地识别数据主体，并查找 Exchange、SharePoint、OneDrive 和 Teams 中组织数据中的个人信息。 

Microsoft Graph权限请求的 API 为组织提供了自动执行重复任务并与现有数据主体请求工具集成的功能，以便能够构建可合并到其业务流程中的可重复工作流。 可以使用主题权限请求 API 来帮助你自动化和扩展组织在 Microsoft 365 中执行主题权限请求搜索的能力，并帮助更有效地满足行业法规。

> [!IMPORTANT]
> 适用于Graph权限请求的 Microsoft Graph API 旨在帮助满足 Exchange Online、SharePoint Online、Teams 聊天和 OneDrive for Business Microsoft 365 服务中的主题权限请求的需求。 这些 API 不应用作在任何其他系统或任何其他区域Microsoft 365搜索数据的替代，因为这些方案不受明确支持。

Microsoft Graph API 包括以下关键实体。

| 名称 | 类型       | 用例 |
|:-|:-|:-|
| 主体权限请求 | [microsoft.graph.subjectRightsRequest](subjectRightsRequest.md) | 表示数据主体正式请求控制者对个人数据采取操作。 |
| 数据主体 | [microsoft.graph.datasubject](datasubject.md) | 包含与内容搜索主题有关的信息。 |
| 主体权限请求历史记录 | [microsoft.graph.subjectRightsRequesthistory](subjectRightsRequesthistory.md) | 表示主题权限请求的历史记录。 |
| 主体权限请求详细信息 | [microsoft.graph.subjectRightsRequestDetail](subjectRightsRequestDetail.md) | 表示主题权限请求的详细信息，包括找到的项目数、审阅的项目数等。 |
| 主体权限请求阶段详细信息 | [microsoft.graph.subjectRightsRequestStageDetail](subjectRightsRequestStageDetail.md) | 表示主题权限请求的阶段的属性。 |

>[!IMPORTANT]
>主题权限请求 API 权限当前不可用。 有关详细信息，请参阅[已知问题](/graph/known-issues#compliance)。

