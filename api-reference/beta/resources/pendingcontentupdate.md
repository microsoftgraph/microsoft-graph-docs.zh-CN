---
title: pendingContentUpdate
description: pendingContentUpdate 资源指示可能影响 driveItem 二进制内容的操作正在等待完成。
ms.localizationpriority: medium
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: notes
doc_type: resourcePageType
ms.openlocfilehash: ec44c2c1d75bc11276d99dad1815c0d999b4f0e1
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176343"
---
# <a name="pendingcontentupdate-resource-type"></a>pendingContentUpdate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示可能影响 **driveItem** 的二进制内容的操作正在等待完成。

## <a name="properties"></a>属性

| 属性     | 类型         | Description |
|:-------------|:-------------|:------------|
|queuedDateTime|DateTimeOffset|挂起的二进制操作在 UTC 时间排队的日期和时间。 只读。|

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


