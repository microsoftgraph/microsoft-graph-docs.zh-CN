---
title: rankedEmailAddress 资源类型
description: 表示排名靠前的电子邮件地址。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: mail
author: AAmatino
ms.openlocfilehash: 2723009cc44680e98b9c8b5a685c06846bb9abd7
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176316"
---
# <a name="rankedemailaddress-resource-type"></a>rankedEmailAddress 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示排名靠前的电子邮件地址。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|string|电子邮件地址。|
|排名|double|电子邮件地址的排名。 与其他返回的结果相比，排名用作排序键。 较高的排名值对应于更相关的结果。 相关性取决于沟通、协作和业务关系信号。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


