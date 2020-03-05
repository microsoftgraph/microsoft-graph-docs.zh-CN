---
title: singleUser 复杂类型
description: 标识租户中将允许作为请求者、审批者或审阅者的用户。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 13792bcffabbc9dceb272cd1cf156fbf9a5a5a10
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520567"
---
# <a name="singleuser-complex-type"></a>singleUser 复杂类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[访问包分配策略](accesspackageassignmentpolicy.md)的请求、审批和分配审阅设置中使用。 `@odata.type`该值`#microsoft.graph.singleUser`指示此用户集标识租户中将允许作为请求者、审批者或审阅者的特定用户。

## <a name="properties"></a>属性

此类型具有以下属性：

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| id |字符串 | Azure AD 中用户的 ID。 |
| 说明 |String | Azure AD 中的用户的名称。 只读。 |
| isBackup | 布尔 | 对于审批阶段的**singleUser** ，指示用户是否为备份回退审批者。 |

## <a name="json-representation"></a>JSON 表示形式

以下是类型的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleUser",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "id": "string (identifier)",
  "description": "string"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleUser complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
