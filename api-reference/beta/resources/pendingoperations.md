---
title: pendingOperations
description: 挂起的Operations 资源指示可能影响 driveItem 状态的一个或多个操作正在等待完成。
ms.localizationpriority: medium
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 6cf3903a99405dbcbdf83f26da053030e46dbb9e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176539"
---
# <a name="pendingoperations-resource-type"></a>pendingOperations 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示可能影响 **driveItem** 状态的一个或多个操作正在等待完成。

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|pendingContentUpdate|[pendingContentUpdate](pendingcontentupdate.md)|一个属性，指示可能更新文件的二进制内容的操作正在等待完成。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingOperations",
  "baseType": null
}-->

```json
{
  "pendingContentUpdate": {"@odata.type": "microsoft.graph.pendingContentUpdate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingOperations resource indicates that an operation that may affect the state of the DriveItem is pending completion.",
  "keywords": "pendingoperations,pendingoperations,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->


