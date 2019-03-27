---
title: freeBusyError 资源类型
description: 表示尝试获取用户、通讯组列表或资源可用性的错误信息。
localization_priority: Normal
ms.openlocfilehash: a08fe8278644ab81f2c1fbe1c7d1530cab27d91b
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2019
ms.locfileid: "30926588"
---
# <a name="freebusyerror-resource-type"></a>freeBusyError 资源类型

表示尝试获取用户、通讯组列表或资源可用性的错误信息。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|message |String |描述错误。 |
|responseCode |字符串 |对用户、通讯组列表或资源的可用性进行查询的响应代码。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
