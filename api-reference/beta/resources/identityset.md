---
author: JeremyKelley
description: identitySet 资源是标识资源的键集合。
title: IdentitySet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
ms.openlocfilehash: 50f6b45c3121f770019d9b5be7e0492242711e1c
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453714"
---
# <a name="identityset-resource-type"></a>identitySet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**identitySet** 资源是标识资源的键 [集合](identity.md)。

它用来表示一组与项目的各种事件相关的标识，例如 _创建者_ 或 _上次修改人_。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "conversation",
    "conversationIdentityType",
    "device",
    "encrypted",
    "guest",
    "phone",
    "user"
  ],
  "openType": true
} -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "microsoft.graph.identity"},
  "conversation": {"@odata.type": "microsoft.graph.identity"},
  "conversationIdentityType": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "encrypted": {"@odata.type": "microsoft.graph.identity"},
  "guest": {"@odata.type": "microsoft.graph.identity"},
  "phone": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>属性

| 属性    | 类型                    | 说明                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| application | [标识](identity.md) | 可选。与此操作关联的应用程序。  |
| conversation| [标识](identity.md) | 可选。 与此操作关联的团队或频道。       |
| conversationIdentityType| [标识](identity.md) | 可选。 指示 conversation **属性是** 标识团队还是频道。|
| 设备      | [标识](identity.md) | 可选。与此操作关联的设备。       |
| phone       | [identity](identity.md) | 可选。 与此操作关联的电话号码。 |
| 用户        | [标识](identity.md) | 可选。与此操作关联的用户。         |

## <a name="remarks"></a>注解 

请参阅 [Call](call.md) for usage of **identitySet** resources。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->


