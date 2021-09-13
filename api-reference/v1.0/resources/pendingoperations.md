---
title: pendingOperations
description: pendingOperations 资源指示可能影响 driveItem 状态的一个或多个操作正在等待完成。
ms.localizationpriority: medium
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 3dd6bccaeadbd98fc28a986f8983c7837a3a8f1d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117905"
---
# <a name="pendingoperations-resource-type"></a>pendingOperations 资源类型

命名空间：microsoft.graph

指示可能影响 **driveItem** 状态的一个或多个操作正在等待完成。

## <a name="properties"></a>属性

| 属性                | 类型        | 说明 |
|:------------------------|:------------|:------------|
|**pendingContentUpdate** |[pendingContentUpdate](pendingcontentupdate.md)|一个属性，指示可能更新文件的二进制内容的操作正在等待完成。|

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

