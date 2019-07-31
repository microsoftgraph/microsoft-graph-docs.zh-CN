---
author: JeremyKelley
description: 共享 资源指示 DriveItem 已与他人共享。
ms.date: 09/10/2017
title: 共享的内容
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d4337341245d355d85d8d4ba74171ed95863e06a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008465"
---
# <a name="shared-resource-type"></a>Shared 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**共享** 资源指示 DriveItem 已与他人共享。此资源包括有关如何共享项的信息。

如果 [**DriveItem**](driveitem.md) 具有非 NULL **共享** facet，则该项已共享。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "scope": "anonymous | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a>属性

| 属性       | 类型                          | 说明
| :------------- |:------------------------------|:----------------------------
| 所有者          | [IdentitySet](identityset.md) | 共享项的所有者的身份。只读。
| scope          | String                        | 指示该项共享方式的范围：`anonymous`、`organization` 或 `users`。只读。
| sharedBy       | [identitySet](identityset.md) | 共享项目的用户的标识。只读。
| sharedDateTime | DateTimeOffset                | 共享项目的 UTC 日期和时间。只读。

## <a name="scope-values"></a>作用域值

| 值          | 说明                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | 使用对任何人都有效的链接共享项。               |
| `organization` | 使用对所有者组织内的任何人都有效的链接共享项。 |
| `users`        | 仅与特定的用户共享项。                                          |

## <a name="remarks"></a>注解

有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。

<!--
{
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared",
  "suppressions": []
}
-->
