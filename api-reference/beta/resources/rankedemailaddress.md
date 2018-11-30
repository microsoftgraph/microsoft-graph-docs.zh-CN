---
title: rankedEmailAddress 资源类型
description: 代表一个排名的电子邮件地址。
ms.openlocfilehash: 9234f527ecba6dc83f2e4f80911442d4a083503a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048311"
---
# <a name="rankedemailaddress-resource-type"></a>rankedEmailAddress 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表一个排名的电子邮件地址。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|string|电子邮件地址。|
|排名|double|电子邮件地址的排名。 排名用作排序关键字，相对于其他返回的结果。 较高的排名值对应于更相关的结果。 相关性取决于沟通、协作和业务关系信号。|

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
<!-- {
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
