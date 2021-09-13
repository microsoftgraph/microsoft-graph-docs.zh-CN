---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 47c3fbe839b5e5f17e76217ca2cda633d8c42c6a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134134"
---
# <a name="workbooksessioninfo-resource-type"></a>workbookSessionInfo 资源类型

命名空间：microsoft.graph

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


