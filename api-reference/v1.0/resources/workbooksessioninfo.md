---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1e9746f27a23b12a3bfdf3168cd271c7f2cbc0d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446690"
---
# <a name="workbooksessioninfo-resource-type"></a>workbookSessionInfo 资源类型

命名空间： microsoft. graph

提供有关工作簿会话的信息。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a>属性

| 属性 | 类型  | 说明                               |
|:---------|:------|:------------------------------------------|
| id  | string | 工作簿会话 的 ID。 |
| persistChanges | boolean |  对于持续会话，值为 `true`。 对于非持续会话（视图模式），值为 `false`。 |

