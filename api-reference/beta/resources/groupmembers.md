---
title: groupMembers 复杂类型
description: 标识租户中将允许作为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 576fd13962dcafaa876225393cc9165e5ef2ece2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078435"
---
# <a name="groupmembers-complex-type"></a>groupMembers 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [访问包分配策略](accesspackageassignmentpolicy.md)的请求、审批和分配审阅设置中使用。 `@odata.type`值 " `#microsoft.graph.groupMembers` " 表示此类型标识租户中将允许作为特定组成员的请求者、审批者或审阅者的用户集合。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| id |String | Azure AD 中的组 ID。 |
| 说明 |String | Azure AD 中的组的名称。 只读。 |
| isBackup | Boolean | 对于审批阶段中的 **groupMembers** ，此属性指示组成员是备份回退审批者。 |

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


