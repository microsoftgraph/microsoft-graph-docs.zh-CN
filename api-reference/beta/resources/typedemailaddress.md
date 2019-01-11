---
title: typedEmailAddress 资源类型
description: 表示的名称、 电子邮件地址和其相应的电子邮件地址类型的联系人。
localization_priority: Normal
ms.openlocfilehash: c77d3dddc3e2bfcac47e6ed245dad9223fe7f08c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871265"
---
# <a name="typedemailaddress-resource-type"></a>typedEmailAddress 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示的名称、 电子邮件地址和其相应的电子邮件地址类型的[联系人](contact.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|String|联系人电子邮件地址。|
|name|字符串|联系人的显示名称。|
|type |字符串 |电子邮件地址类型。 可取值为：`unknown`、`work`、`personal`、`main`、`other`。 默认值是`unknown`，这意味着**地址**尚未设置为特定的类型。 |
|otherLabel |字符串  |若要指定自定义类型的电子邮件地址，请将**类型**设置为`other`，并将**otherLabel**分配给自定义字符串。 例如，您可以使用特定的电子邮件地址您自愿活动。 **类型**设置为`other`，如设置为自定义字符串**otherLabel** `Volunteer work`。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
