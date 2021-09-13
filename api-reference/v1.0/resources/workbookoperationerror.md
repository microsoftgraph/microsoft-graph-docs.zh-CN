---
title: workbookOperationError 资源类型
description: 表示失败的工作簿操作中的错误。
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: aeddf940bfbbc9fdd7bba44afcd34990ffd7b671
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139434"
---
# <a name="workbookoperationerror-resource-type"></a>workbookOperationError 资源类型

表示失败的工作簿操作中的错误。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|code|String| 错误代码。|
|message|String| 错误消息。|
|innererror|error object| 可选。可能比顶级错误更具体的其他错误对象。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperationError",
  "baseType": null
}-->

```json
{
  "code": "String",
  "message": "String",
  "innererror": { "@odata.type": "odata.error" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

