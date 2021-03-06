---
title: singleUser 复杂类型
description: 标识租户中将允许其成为请求者、审批者或审阅者的用户。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8e1982eef048e1f68f579df7f2ebc6b0975f2f0b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761042"
---
# <a name="singleuser-complex-type"></a>singleUser 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在访问包分配策略的请求、审批和分配审阅 [设置中使用](accesspackageassignmentpolicy.md)。 该值指示此用户集标识租户中将允许其成为请求者、审批者或审阅者  `@odata.type` `#microsoft.graph.singleUser` 的特定用户。

## <a name="properties"></a>属性

此类型具有以下属性：

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| id |String | Azure AD 中的用户 ID。 |
| 说明 |String | Azure AD 中的用户名。 只读。 |
| isBackup | 布尔 | 对于 **审批阶段中的 singleUser，** 指示用户是否是备份回退审批者。 |

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


