---
title: 使用 Microsoft Graph 记录管理 API
description: Microsoft Purview 记录管理 API 可帮助组织管理数据的保留和删除，以满足其法律义务和合规性法规，并通过允许定期处置不再需要保留的项目来提高效率。
ms.localizationpriority: medium
author: sseth-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: 0c977e56c8c3cb70f2e6ee2fab17d80daff8a7be
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609680"
---
# <a name="use-the-microsoft-graph-records-management-apis"></a>使用 Microsoft Graph 记录管理 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Purview 记录管理 API 可帮助组织管理数据的保留和删除，以满足其法律义务和合规性法规，并通过允许定期处置不再需要保留的项目来提高效率。

记录管理解决方案是 Microsoft Purview 合规中心的一部分。

## <a name="manage-retention-labels"></a>管理保留标签
记录管理管理员和开发人员需要使用定期创建、更新和删除的标签来维护记录管理系统。

开发人员和合规性管理员可以使用记录管理 API 对记录管理标签执行操作，以维护其系统。

## <a name="trigger-events-for-an-existing-label"></a>触发现有标签的事件
当员工离开公司时，信息会在 HR 管理系统中更新。 从休假日期起，机密文件需要保留 7 年。 这些文档已应用标签 `Employee_departure` 。

开发人员和合规性管理员可以使用记录管理 API 读取标签 `Employee_departure` 并查找关联的事件类型 `Event-employee_departure`。

合规性管理员可以使用记录管理 API 为关联的事件类型创建事件。 机密文档的保留期在创建此事件后开始。

## <a name="entities"></a>实体
记录管理 API 包括以下关键实体。

| 名称 | 类型       | 用例 |
|:-|:-|:-|
| 标签 | [microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md) | 包含可在句点结束时应用于项的保留设置和操作。 |
| 保留事件 | [microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md) | 表示基于事件的保留的触发器，其中保留期在事件发生后开始。 |
| 保留事件类型 | [microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md) | 表示相同类型的保留事件的单个组。 |
