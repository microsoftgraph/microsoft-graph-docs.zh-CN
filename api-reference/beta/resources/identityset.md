---
author: JeremyKelley
description: 了解 identityset 资源是标识资源的键控集合。
ms.date: 09/10/2017
title: 了解 identityset
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 08986af20ae7591798a222e68d9b9bee5244e273
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496605"
---
# <a name="identityset-resource-type"></a>了解 identityset 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**了解 identityset**资源是[标识](identity.md)资源的键控集合。

它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。

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
| 对话| [标识](identity.md) | 可选。 与此操作关联的团队或频道。       |
| conversationIdentityType| [标识](identity.md) | 可选。 指示**会话**属性是否标识团队或频道。|
| 设备      | [标识](identity.md) | 可选。与此操作关联的设备。       |
| phone       | [identity](identity.md) | 可选。 与此操作关联的电话号码。 |
| 用户        | [标识](identity.md) | 可选。与此操作关联的用户。         |

## <a name="remarks"></a>注解 

有关**了解 identityset**资源的使用情况，请参阅[Call](call.md) 。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
