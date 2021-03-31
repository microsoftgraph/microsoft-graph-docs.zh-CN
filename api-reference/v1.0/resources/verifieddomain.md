---
title: verifiedDomain 资源类型
description: 指定租户的域。 **organization 实体的 verifiedDomains** 属性是 **VerifiedDomain 的集合**。
localization_priority: Normal
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8636552fa99b3389f35f22e2edccc5d13cb06482
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468980"
---
# <a name="verifieddomain-resource-type"></a>verifiedDomain 资源类型

命名空间：microsoft.graph

指定租户的域。 **organization 实体的 verifiedDomains** 属性是 **VerifiedDomain 的集合**。 [](organization.md)


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

