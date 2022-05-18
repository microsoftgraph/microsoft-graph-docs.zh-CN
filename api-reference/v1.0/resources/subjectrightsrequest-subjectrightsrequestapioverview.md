---
title: 使用 Microsoft Graph主题权限请求 API
description: 使用者权限请求 API 为组织提供了自动执行重复性任务的功能，并与其现有的主体权限请求工具集成，以生成可重复的工作流，以帮助满足行业法规的要求。
ms.localizationpriority: medium
author: skadam-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: 0d156730d1ec71376a853d3df9139669e094f9b0
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461182"
---
# <a name="use-the-microsoft-graph-subject-rights-request-api"></a>使用 Microsoft Graph主题权限请求 API

根据世界各地的某些隐私法规，个人可以请求查看或管理公司收集的有关自己的个人数据。 这些请求在Microsoft Priva解决方案中称为主题权限请求;它们有时也称为数据主体请求 (DSR) 或数据主体访问请求 (DSAR) 。 Microsoft Priva使负责满足主体权利请求的人员能够轻松识别数据主体，并在组织的数据中查找其个人信息，Exchange、SharePoint、OneDrive和Teams。 

使用者权限请求的 Microsoft Graph API 为组织提供了自动执行重复任务和与现有数据主体请求工具集成的功能，以启用可合并到其业务流程的可重复工作流。 可以使用主题权限请求 API 来帮助你自动化和扩展组织在Microsoft 365中执行主题权限请求搜索的能力，并帮助更高效地满足行业法规。

> [!IMPORTANT]
> 适用于主题权限请求的 Microsoft Graph API 旨在帮助满足满足Exchange Online、SharePoint联机、Teams聊天和OneDrive for Business Microsoft 365服务中的主体权限请求的需求。 这些 API 不应用作在任何其他Microsoft 365系统或任何其他区域中搜索数据的替代项，因为这些方案不受显式支持。

Microsoft Graph API 包括以下关键实体。

| 名称 | 类型       | 用例 |
|:-|:-|:-|
| 使用者权限请求 | [microsoft.graph.subjectRightsRequest](subjectRightsRequest.md) | 表示受控制器要求对其个人数据执行操作的数据的正式请求。 |
| 数据主体 | [microsoft.graph.datasubject](datasubject.md) | 包含与内容搜索主题相关的信息。 |
| 使用者权限请求历史记录 | [microsoft.graph.subjectRightsRequesthistory](subjectRightsRequesthistory.md) | 表示主题权限请求的历史记录。 |
| 主题权限请求详细信息 | [microsoft.graph.subjectRightsRequestDetail](subjectRightsRequestDetail.md) | 表示主题权限请求的详细信息，包括找到的项目数、审阅的项目数等。 |
| 主题权限请求阶段详细信息 | [microsoft.graph.subjectRightsRequestStageDetail](subjectRightsRequestStageDetail.md) | 表示主题权限请求的各个阶段的属性。 |


