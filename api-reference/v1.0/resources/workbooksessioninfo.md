---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
ms.openlocfilehash: 84d0306a7a25aaa29e4f1eb9b87708cc97d6b50f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009514"
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

