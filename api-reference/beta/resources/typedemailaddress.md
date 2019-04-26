---
title: typedEmailAddress 资源类型
description: 表示联系人的名称、电子邮件地址及其对应的电子邮件地址类型。
localization_priority: Normal
ms.openlocfilehash: 92f3f1f89c73fe968c7fb06f7c5ed4b0eff883fa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345468"
---
# <a name="typedemailaddress-resource-type"></a>typedEmailAddress 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[联系人](contact.md)的名称、电子邮件地址及其对应的电子邮件地址类型。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|String|联系人的电子邮件地址。|
|name|字符串|联系人的显示名称。|
|type |String |电子邮件地址的类型。 可取值为：`unknown`、`work`、`personal`、`main`、`other`。 默认值为`unknown`, 表示尚未将**地址**设置为特定类型。 |
|otherLabel |String  |若要指定自定义类型的电子邮件地址**** , 请`other`将 "类型" 设置为, 并将**otherLabel**分配给自定义字符串。 例如, 您可以对志愿者活动使用特定的电子邮件地址。 将**** "类型`other`" 设置为, 并将**otherLabel**设置为自`Volunteer work`定义字符串, 例如。 |

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
