---
title: commsNotification 资源类型
description: 通信服务器发布的用于通知更改的通信通知基本类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ff7d46a6d081889897940a93d5d111ffa2956a21fc61411060cad08ed2f7d5ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252016"
---
# <a name="commsnotification-resource-type"></a>commsNotification 资源类型

命名空间：microsoft.graph

通信服务器发布的用于通知更改的通信通知基本类型。

## <a name="properties"></a>属性
| 属性       | 类型    | 说明                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| changeType     | String  | 可取值为：`created`、`updated`、`deleted`。      |
| resourceUrl       | String  | 已更改资源的 URI。                      |

> **注意：** `resourceData` 作为其他数据提供。 它是实体或实体集合，具体取决于通知中打包的更改数。

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

