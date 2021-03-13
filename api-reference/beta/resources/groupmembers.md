---
title: groupMembers 复杂类型
description: 标识租户中将允许其成为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0069cd6a8fd738c17a9035b519c4f141c3a5fa55
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761414"
---
# <a name="groupmembers-complex-type"></a>groupMembers 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在访问包分配策略的请求、审批和分配审阅 [设置中使用](accesspackageassignmentpolicy.md)。 值" " 指示此类型标识租户中将允许作为请求者、审批者或审阅者的用户集合，这些用户是特定 `@odata.type` `#microsoft.graph.groupMembers` 组的成员。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| id |String | Azure AD 中组的 ID。 |
| 说明 |String | Azure AD 中的组名称。 只读。 |
| isBackup | 布尔 | 对于 **处于审批阶段的 groupMembers，** 此属性指示该组的成员是备份回退审批者。 |

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
  "id": "string (identifier)",
  "description": "string",
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


