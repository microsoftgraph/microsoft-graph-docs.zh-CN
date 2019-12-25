---
title: resultInfo 资源类型
description: 这包含成功和失败的特定结果信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 39027ecf949860d9ffa757a95839ae7fd8184a27
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865766"
---
# <a name="resultinfo-resource-type"></a>resultInfo 资源类型

这包含成功和失败的特定结果信息。 

该代码指定结果是否为一般性成功或失败。 如果代码是2xx，如果它是一个客户端错误，它是成功的，如果是5xx，则表示服务器出错。

子代码提供与成功或失败类型相关的补充信息（例如，呼叫转移成功）


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
