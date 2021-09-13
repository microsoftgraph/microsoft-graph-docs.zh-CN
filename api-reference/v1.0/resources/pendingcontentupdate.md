---
title: pendingContentUpdate
description: pendingContentUpdate 资源指示可能影响 driveItem 的二进制内容的操作正在等待完成。
ms.localizationpriority: medium
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: d472ba41c26885bdefad13f35ea66f7b4e974d6a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117932"
---
# <a name="pendingcontentupdate-resource-type"></a>pendingContentUpdate 资源类型

命名空间：microsoft.graph

指示可能影响 **driveItem** 的二进制内容的操作正在等待完成。

## <a name="properties"></a>属性

| 属性     | 类型         | 说明 |
|:-------------|:-------------|:------------|
|**queuedDateTime**|DateTimeOffset|挂起的二进制操作在 UTC 时间排队的日期和时间。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingContentUpdate",
  "baseType": null
}-->

```json
{
  "queuedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingContentUpdate resource indicates that an operation that may affect the binary content of the DriveItem is pending completion.",
  "keywords": "pendingoperation,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->

