---
title: targetResourceUser 资源类型
description: 指示已添加、 更新或删除管理员审核活动的一部分的用户对象。 派生 targetResource 资源。
ms.openlocfilehash: 632d0551b3aba434c3309c8c874947708eb9a9f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044761"
---
# <a name="targetresourceuser-resource-type"></a>targetResourceUser 资源类型
指示已添加、 更新或删除管理员审核活动的一部分的用户对象。 派生[targetResource](targetresource.md)资源。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|userPrincipalName|字符串|指示用户的唯一 Id。 为某个特定用户是指用户 Id。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceUser"
}-->

```json
{
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->