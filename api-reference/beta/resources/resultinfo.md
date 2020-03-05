---
title: resultInfo 资源类型
description: 包含成功和失败的特定结果信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aa55f8cdcb7ca4639aa4975a28ae2bcbcd625588
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521080"
---
# <a name="resultinfo-resource-type"></a>resultInfo 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含成功和失败的特定结果信息。 

该代码指定结果是否为一般性成功或失败。 

子代码提供与成功或失败类型相关的补充信息（例如，呼叫转移成功）。


## <a name="properties"></a>属性

| 属性 | 类型   | 说明          |
| :------- | :----- | :------------------  |
| code     | Int32 | 结果代码。     |
| message  | String | 邮件。         |
| subcode  | Int32 | 结果子代码。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": 0,
  "message": "String",
  "subcode": 0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
