---
title: verifiedDomain 资源类型
description: 指定租户的域。 组织实体的**verifiedDomains**属性是**VerifiedDomain**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 63e1f2af238aa05fbe5918ff3fc54b5a292aef21
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519482"
---
# <a name="verifieddomain-resource-type"></a>verifiedDomain 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定租户的域。 [组织](organization.md)实体的**VerifiedDomains**属性是**VerifiedDomain**的集合。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|capabilities|String|例如，“Email”、“OfficeCommunicationsOnline”。|
|isDefault|布尔|                如果这是与租户关联的默认域，则为 **true**；否则为 **false**。            |
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
<!--
{
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
