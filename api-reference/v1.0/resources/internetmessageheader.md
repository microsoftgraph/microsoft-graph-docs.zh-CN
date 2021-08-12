---
title: internetMessageHeader 资源类型
description: '一个键值对，表示由 RFC5322 定义的 Internet 邮件头，该键值对提供 '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a1b3fbc979c8374b8f4c48b96ebe5dfc31b22cc5dd2849f686528d1a4e84cf06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218693"
---
# <a name="internetmessageheader-resource-type"></a>internetMessageHeader 资源类型

命名空间：microsoft.graph


一个键值对，它表示 Internet 邮件头，正如 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 所定义的那样，它提供邮件获取的从发件人到收件人的网络路径的详细信息。

有关 Internet 邮件头示例，请参阅[查看电子邮件头](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4)。


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
<!-- {
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

