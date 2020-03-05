---
title: commsNotification 资源类型
description: 通信服务器发布的用于通知更改的通信通知基类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4ec3df8bc56e6164af3b7752333d28bd10665d67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507602"
---
# <a name="commsnotification-resource-type"></a>commsNotification 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通信服务器发布的用于通知更改的通信通知基类型。

## <a name="properties"></a>属性
| 属性       | 类型    | 说明                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| changeType     | String  | 可取值为：`created`、`updated`、`deleted`。      |
| resourceUrl       | String  | 已更改的资源的 URI。                      |

> **注意：** `resourceData`可用作其他数据。 它可以是实体，也可以是实体集合，具体取决于通知中打包的更改数。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "resourceData"
  ],
  "@odata.type": "microsoft.graph.commsNotification",
  "openType": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotification",
  "changeType": "created | updated | deleted",
  "resourceUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
