---
title: userSet 复杂类型
description: 访问包分配策略的请求、审批和分配审阅设置中使用的类型的抽象基类型。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 77f0f990587531c10914644366e066a0fd659f37
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519503"
---
# <a name="userset-complex-type"></a>userSet 复杂类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[访问包分配策略](accesspackageassignmentpolicy.md)的请求、审批和分配审阅设置中使用。 [SingleUser](singleuser.md)、[groupMembers](groupmembers.md)、 [connectedOrganizationMembers](connectedorganizationmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md)和[externalSponsors](externalsponsors.md)类型的抽象基类型。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | 布尔 | 对于审批阶段中的用户，此属性指示用户是否为备份回退审批者。 |

## <a name="json-representation"></a>JSON 表示形式

以下是 userSet 的 JSON 表示形式。  请注意，userSet 是抽象基类，因此不会发送或接收。  而是将使用 " `@odata.type` `#microsoft.graph.singleUser``#microsoft.graph.groupMembers`"、""、"`#microsoft.graph.connectedOrganizationMembers`"、"`#microsoft.graph.requestorManager`"、`#microsoft.graph.internalSponsors`"" 或 "`#microsoft.graph.externalSponsors`" 中的一个。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet",
  "baseType": ""
}-->

```json
{
       "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSet complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
