---
title: freeBusyError 资源类型
description: 表示尝试获取用户、通讯组列表或资源的可用性的错误信息。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 16bb344b432c6c5e911635ad2d8e3d2f61c1c32b2faa9f5fb167ce28028aeeef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216908"
---
# <a name="freebusyerror-resource-type"></a>freeBusyError 资源类型

命名空间：microsoft.graph

表示尝试获取用户、通讯组列表或资源的可用性的错误信息。

## <a name="properties"></a>属性
| 属性     | 类型   |描述|
|:---------------|:--------|:----------|
|message |String |描述错误。 |
|responseCode |String |查询用户、通讯组列表或资源的可用性的响应代码。 |


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

