---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: b0ee801945a4b1d202b55d997d8cfc87a8dadff5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829153"
---
# <a name="identityset-resource-type"></a>IdentitySet 资源类型

**IdentitySet** 资源是 [标识](identity.md) 资源的键控集合。它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identitySet",
       "optionalProperties": ["user", "application", "device"],
       "openType": true } -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>属性

| 属性    | 类型                    | 说明                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| application | [标识](identity.md) | 可选。与此操作关联的应用程序。 |
| 设备      | [标识](identity.md) | 可选。与此操作关联的设备。      |
| 用户        | [标识](identity.md) | 可选。与此操作关联的用户。        |

## <a name="remarks"></a>注解 

请参阅 [DriveItem](driveitem.md) 以了解 **IdentitySet** 资源的使用情况。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
