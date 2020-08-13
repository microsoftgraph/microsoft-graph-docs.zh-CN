---
title: pendingContentUpdate
description: PendingContentUpdate 资源指示可能影响 driveItem 的二进制内容的操作处于 "正在等待" 已完成。
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7862d8da186448d08d6dfd5691ae83e29bd57a5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521974"
---
# <a name="pendingcontentupdate-resource-type"></a>pendingContentUpdate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示可能会影响**driveItem**的二进制内容的操作正在等待完成。

## <a name="properties"></a>属性

| 属性     | 类型         | 说明 |
|:-------------|:-------------|:------------|
|queuedDateTime|DateTimeOffset|在 UTC 时间内排队待执行的二进制操作的日期和时间。 只读。|

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
