---
title: resultInfo 资源类型
description: 其中包含特定于成功和失败的结果信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 37a6d7a1881a26d79df568b2fa8f81382ae8b32089ea7683d003522b82805b8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54177980"
---
# <a name="resultinfo-resource-type"></a>resultInfo 资源类型

命名空间：microsoft.graph

其中包含特定于成功和失败的结果信息。 

该代码指定结果是一般成功还是失败。 如果代码为 2xx，则成功，如果是 4xx，则它是客户端错误，如果是 5xx，则说明服务器错误。

子代码提供与成功或失败类型相关的补充信息 (例如呼叫转接成功) 


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

