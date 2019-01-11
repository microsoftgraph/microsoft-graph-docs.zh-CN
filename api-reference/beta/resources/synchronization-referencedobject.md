---
title: referencedObject 资源类型
description: 介绍在相同的目录定义中定义的另一个对象的引用。
localization_priority: Normal
ms.openlocfilehash: 5a2aa2dcc358c856c18ea2ce9871ec634194ce54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821033"
---
# <a name="referencedobject-resource-type"></a>referencedObject 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

介绍在相同的[目录定义](synchronization-directorydefinition.md)中定义的另一个对象的引用。

## <a name="properties"></a>属性

| 属性                   | 类型                      | Description    |
|:---------------------------|:--------------------------|:---------------|
|referencedObjectName        |字符串                     |引用对象的名称。 必须匹配一个[目录定义](synchronization-directorydefinition.md)中的对象。|
|referencedProperty          |字符串                     |**当前不支持**。 中引用的对象，其中的值用作引用的属性的名称。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
            
