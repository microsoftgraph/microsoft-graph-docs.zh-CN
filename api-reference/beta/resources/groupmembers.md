---
title: groupMembers 复杂类型
description: 标识租户中将允许作为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b4170a3baf186d907340bc1c490c508644ec30a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496934"
---
# <a name="groupmembers-complex-type"></a>groupMembers 复杂类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[访问包分配策略](accesspackageassignmentpolicy.md)的请求、审批和分配审阅设置中使用。 `@odata.type`值 "`#microsoft.graph.groupMembers`" 表示此类型标识租户中将允许作为特定组成员的请求者、审批者或审阅者的用户集合。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| id |字符串 | Azure AD 中的组 ID。 |
| 说明 |String | Azure AD 中的组的名称。 只读。 |
| isBackup | 布尔 | 对于审批阶段中的**groupMembers** ，此属性指示组成员是备份回退审批者。 |

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
