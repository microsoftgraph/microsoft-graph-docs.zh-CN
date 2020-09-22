---
title: typedEmailAddress 资源类型
description: 表示联系人的名称、电子邮件地址及其对应的电子邮件地址类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: 8ce8ebdd0cb5b8b2113a80dacf72617d0f361356
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993006"
---
# <a name="typedemailaddress-resource-type"></a>typedEmailAddress 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [联系人](contact.md)的名称、电子邮件地址及其对应的电子邮件地址类型。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|String|联系人的电子邮件地址。|
|name|String|联系人的显示名称。|
|type |String |电子邮件地址的类型。 可取值为：`unknown`、`work`、`personal`、`main`、`other`。 默认值为 `unknown` ，表示尚未将 **地址** 设置为特定类型。 |
|otherLabel |String  |若要指定自定义类型的电子邮件地址，请将 " **类型** " 设置为 `other` ，并将 **otherLabel** 分配给自定义字符串。 例如，您可以对志愿者活动使用特定的电子邮件地址。 将 " **类型** " 设置为 `other` ，并将 **otherLabel** 设置为自定义字符串，例如 `Volunteer work` 。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
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


