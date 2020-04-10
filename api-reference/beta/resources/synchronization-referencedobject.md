---
title: referencedObject 资源类型
description: 描述对在同一目录定义中定义的另一个对象的引用。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7779fb851812c00c15749877517b79273752ab58
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217589"
---
# <a name="referencedobject-resource-type"></a>referencedObject 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述对在同一[目录定义](synchronization-directorydefinition.md)中定义的另一个对象的引用。

## <a name="properties"></a>属性

| 属性                   | 类型                      | 说明    |
|:---------------------------|:--------------------------|:---------------|
|referencedObjectName        |字符串                     |引用的对象的名称。 必须与[目录定义](synchronization-directorydefinition.md)中的一个对象相匹配。|
|referencedProperty          |字符串                     |**目前不支持**。 引用的对象中属性的名称，其值将用作引用。|

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
<!--
{
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
            
