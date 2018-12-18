---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
author: lumine2008
ms.openlocfilehash: 1e097cad70a6058aab28ad85d7cf6b3c3b52ac75
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305983"
---
# <a name="workbooksessioninfo-resource-type"></a>workbookSessionInfo 资源类型

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
| ID  | string | 工作簿会话 的 ID。 |
| persistChanges | boolean |  对于持续会话，值为 `true`。 对于非持续会话（视图模式），值为 `false`。 |

