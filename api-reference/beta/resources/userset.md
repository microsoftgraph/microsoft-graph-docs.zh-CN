---
title: userSet 复杂类型
description: 访问包分配策略的请求、审批和分配审阅设置中使用的类型的抽象基类型。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 541bce7c65eaa9b284e9da5b520913b1be4ca8a3
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777712"
---
# <a name="userset-complex-type"></a>userSet 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于访问包分配策略的请求、审批和 [分配审阅设置](accesspackageassignmentpolicy.md)。 singleUser、groupMembers、connectedOrganizationMembers、requestorManager、internalSponsors[](internalsponsors.md)和[externalSponsors](externalsponsors.md)类型的抽象基类型。 [](singleuser.md)[](groupmembers.md) [](connectedorganizationmembers.md) [](requestormanager.md)

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | 布尔值 | 对于处于审批阶段的用户，此属性指示用户是否是备份回退审批者。 |

## <a name="json-representation"></a>JSON 表示形式

下面是 userSet 的 JSON 表示形式。  请注意，userSet 是抽象基类，因此不会发送或接收。  而是使用" `@odata.type` `#microsoft.graph.singleUser` "， " `#microsoft.graph.groupMembers` "， " `#microsoft.graph.connectedOrganizationMembers` 或 `#microsoft.graph.requestorManager` " `#microsoft.graph.internalSponsors` `#microsoft.graph.externalSponsors` 之一。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet"
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


