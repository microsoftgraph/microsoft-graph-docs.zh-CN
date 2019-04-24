---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 502781c4049c9451f5ed67ff97222abf4df462d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456834"
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
| id  | string | 工作簿会话 的 ID。 |
| persistChanges | 布尔 |  对于持续会话，值为 `true`。 对于非持续会话（视图模式），值为 `false`。 |

