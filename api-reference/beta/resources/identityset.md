---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 了解 identityset
localization_priority: Normal
ms.openlocfilehash: 0a963f7158dbb812fc1f51fbff208297a2a9f076
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482194"
---
# <a name="identityset-resource-type"></a>了解 identityset 资源类型

**IdentitySet** 资源是 [标识](identity.md) 资源的键控集合。它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
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
  "application": {"@odata.type": "#microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "#microsoft.graph.identity"},
  "device": {"@odata.type": "#microsoft.graph.identity"},
  "encrypted": {"@odata.type": "#microsoft.graph.identity"},
  "guest": {"@odata.type": "#microsoft.graph.identity"},
  "phone": {"@odata.type": "#microsoft.graph.identity"},
  "user": {"@odata.type": "#microsoft.graph.identity"}
}
```

## <a name="properties"></a>属性

| 属性    | 类型                    | 说明                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| application | [Identity](identity.md) | 可选。与此操作关联的应用程序。  |
| 设备      | [Identity](identity.md) | 可选。与此操作关联的设备。       |
| phone       | [identity](identity.md) | 可选。 与此操作关联的电话号码。 |
| 用户        | [标识](identity.md) | 可选。与此操作关联的用户。         |

## <a name="remarks"></a>注解 

有关**了解 identityset**资源的使用情况, 请参阅[Call](call.md) 。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
