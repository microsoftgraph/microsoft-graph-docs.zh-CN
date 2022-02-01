---
title: internetMessageHeader 资源类型
description: '一个键值对，表示由 RFC5322 定义的 Internet 邮件头，它提供 '
ms.localizationpriority: medium
doc_type: resourcePageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: 5c17023185261b86a53eb87eccc5fce8be8df1d1
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291167"
---
# <a name="internetmessageheader-resource-type"></a>internetMessageHeader 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个键值对，它表示 Internet 邮件头，正如 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 所定义的那样，它提供邮件获取的从发件人到收件人的网络路径的详细信息。

有关 Internet 邮件头示例，请参阅[查看电子邮件头](https://support.office.com/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4)。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|name|string|表示键值对中的键。|
|value|string|键值对中的值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


