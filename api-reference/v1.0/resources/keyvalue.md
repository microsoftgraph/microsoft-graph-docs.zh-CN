---
title: keyValue 资源类型
description: 标准键值对资源类型。
localization_priority: Normal
author: dougeby
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 226d27e73a3a253ab7988f74f05fa6377cae1c6d997e16e17e73fc4698c85529
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163724"
---
# <a name="keyvalue-resource-type"></a>keyValue 资源类型

命名空间：microsoft.graph

表示键值对。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|Key|string| 键值对的键。 |
|value|string| 键值对的值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValue"
}-->

```json
{
  "key": "string",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

