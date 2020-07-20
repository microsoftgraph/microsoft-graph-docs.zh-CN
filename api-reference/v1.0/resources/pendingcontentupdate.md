---
title: pendingContentUpdate
description: PendingContentUpdate 资源指示可能影响 driveItem 的二进制内容的操作处于 "正在等待" 已完成。
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: b1a197ae60dc8bb60533d567c6472a65988c3962
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863801"
---
# <a name="pendingcontentupdate-resource-type"></a>pendingContentUpdate 资源类型

命名空间：microsoft.graph

指示可能会影响**driveItem**的二进制内容的操作正在等待完成。

## <a name="properties"></a>属性

| 属性     | 类型         | 说明 |
|:-------------|:-------------|:------------|
|**queuedDateTime**|DateTimeOffset|在 UTC 时间内排队待执行的二进制操作的日期和时间。 只读。|

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
