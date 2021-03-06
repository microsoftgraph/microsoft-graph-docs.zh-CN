---
author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
description: IdentitySet 资源是 标识 资源的键控集合。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e6f7aef915596e39173f286a3433e0114656e707
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239959"
---
# <a name="identityset-resource-type"></a>IdentitySet 资源类型

命名空间：microsoft.graph

**IdentitySet** 资源是 [标识](identity.md) 资源的键控集合。它用来表示一组与项目的各种事件相关的标识，例如 _创建者_ 或 _上次修改人_。

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

