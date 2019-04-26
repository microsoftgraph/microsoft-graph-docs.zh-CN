---
title: emailAddress 资源类型
description: 表示实体实例的名称和 SMTP 地址, 例如, 邮件收件人或日历所有者。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e8b49e0ff502f6e36e6ca3291d675c839e9ff5e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340303"
---
# <a name="emailaddress-resource-type"></a>emailAddress 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示实体实例的名称和 SMTP 地址, 例如, 邮件收件人或日历所有者。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|String|实体实例的电子邮件地址。|
|name|String|实体实例的显示名称。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
