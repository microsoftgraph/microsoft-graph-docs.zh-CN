---
title: 使用 Microsoft Graph权限请求 API
description: 此Microsoft 365权限请求 API 为组织提供了自动执行重复任务并与现有主体权限请求工具集成的功能，以构建可重复的工作流，帮助满足行业法规。
ms.localizationpriority: medium
author: skadam-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: 772134d7574011d2bd5695b07abf5aa5cd1d3348
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861206"
---
# <a name="use-the-microsoft-graph-subject-rights-request-api"></a>使用 Microsoft Graph权限请求 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

根据全球的某些隐私法规，个人可以请求查看或管理公司收集的有关自己的个人数据。 这些请求在 Microsoft 365 隐私管理解决方案中称为主体权限请求;它们有时也称为数据主体请求 (DSR) 或数据主体访问请求 (DSAR) 。 Microsoft 365隐私管理使负责履行主体权利请求的人员能够轻松地识别数据主体，并查找 Exchange、SharePoint、OneDrive 和 Teams 中组织数据中的个人信息。 

Microsoft Graph主题权限请求 API 为组织提供了自动执行重复任务并与现有数据主体请求工具集成的功能，以便能够构建可合并到其业务流程中的可重复工作流。 可以使用主题权限请求 API 来帮助自动执行和扩展组织在 Microsoft 365 中执行主题权限请求搜索的能力，并帮助更有效地满足行业法规。

> [!IMPORTANT]
> 适用于Graph权限请求的 Microsoft Graph API 旨在帮助满足在 Microsoft 365 服务中为 Exchange Online、SharePoint Online、Teams 聊天和 OneDrive for Business 实现主题权限请求的需求。 这些 API 不应用作在任何其他系统或任何其他区域Microsoft 365搜索数据的替代，因为这些方案不受明确支持。

Microsoft Graph API 包括以下关键实体。

| 名称 | 类型       | 用例 |
|:-|:-|:-|
| 使用者权限请求 | [microsoft.graph.subjectRightsRequest](subjectRightsRequest.md) | 表示数据主体正式请求控制者对个人数据采取操作。 |
| 数据主体 | [microsoft.graph.datasubject](datasubject.md) | 包含与内容搜索主题有关的信息。 |
| 主体权限请求历史记录 | [microsoft.graph.subjectRightsRequesthistory](subjectRightsRequesthistory.md) | 表示主题权限请求的历史记录。 |
| 主体权限请求详细信息 | [microsoft.graph.subjectRightsRequestDetail](subjectRightsRequestDetail.md) | 表示主题权限请求的详细信息，包括找到的项目数、审阅的项目数等。 |
| 主体权限请求阶段详细信息 | [microsoft.graph.subjectRightsRequestStageDetail](subjectRightsRequestStageDetail.md) | 表示主题权限请求的阶段的属性。 |




