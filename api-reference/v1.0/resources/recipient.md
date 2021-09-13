---
title: 收件人资源类型
description: '表示事件、邮件或组帖子发送或接收端的用户的相关信息。 '
ms.localizationpriority: medium
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a484a49e582d2df904dde65572453836b9d2fc4a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078663"
---
# <a name="recipient-resource-type"></a>收件人资源类型

命名空间：microsoft.graph

表示事件、邮件或组帖子发送或接收端的用户的相关信息。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|emailAddress|[EmailAddress](emailaddress.md)|收件人的电子邮件地址。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

