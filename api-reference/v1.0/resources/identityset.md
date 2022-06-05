---
author: JeremyKelley
title: identitySet 资源类型
ms.localizationpriority: medium
description: 表示标识资源的密钥集合。
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 3f91b44dd10d842787aba9af96fa57a4ef67f53b
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899937"
---
# <a name="identityset-resource-type"></a>identitySet 资源类型

命名空间：microsoft.graph

**identitySet** 资源是 [标识](identity.md)资源的密钥集合。
它用来表示一组与项目的各种事件相关的标识，例如 _创建者_ 或 _上次修改人_。

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

有关 **identitySet** 资源的使用情况，请参阅 [driveItem](driveitem.md)。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->

