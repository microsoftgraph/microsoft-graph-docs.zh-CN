---
title: groupMembers 复杂类型
description: 标识租户中将允许其成为请求者、审批者或审阅者的用户的集合。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ce18ed739e1701e004c92f408d0276ef17f5d264
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2021
ms.locfileid: "60289957"
---
# <a name="groupmembers-complex-type"></a>groupMembers 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在访问包分配策略的请求、审批和分配审阅 [设置中使用](accesspackageassignmentpolicy.md)。 该值指示此类型标识租户中将允许作为请求者、审批者或审阅者的用户的集合，这些用户是特定 `@odata.type` `#microsoft.graph.groupMembers` 组的成员。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| id |字符串 | 组中组的 ID Azure AD。 |
| 说明 |字符串 | 组中组的名称Azure AD。 只读。 |
| isBackup | Boolean | 对于 **处于审批阶段的 groupMembers，** 此属性指示该组的成员是备份回退审批者。 |

## <a name="json-representation"></a>JSON 表示形式


以下是类型的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


