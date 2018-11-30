---
title: verifiedDomain 资源类型
description: 指定租户的域。组织 实体的 **verifiedDomains** 属性是一个 **VerifiedDomain** 集合。
ms.openlocfilehash: 21b6dd89dcc8b990046952d9ae7abcfe8ce02bca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008981"
---
# <a name="verifieddomain-resource-type"></a>verifiedDomain 资源类型

指定租户的域。[组织](organization.md) 实体的 **verifiedDomains** 属性是一个 **VerifiedDomain** 集合。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|capabilities|String|例如，“Email”、“OfficeCommunicationsOnline”。|
|isDefault|Boolean|                如果这是与租户关联的默认域，则为 **true**；否则为 **false**。            |
|isInitial|Boolean|如果这是与租户关联的初始域，则为 **true**；否则为 **false**|
|name|String|域名；例如，“contoso.onmicrosoft.com”|
|type|String|例如，“Managed”。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
