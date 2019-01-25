---
title: typedEmailAddress 资源类型
description: 表示的名称、 电子邮件地址和其相应的电子邮件地址类型的联系人。
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510706"
---
# <a name="typedemailaddress-resource-type"></a>typedEmailAddress 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示的名称、 电子邮件地址和其相应的电子邮件地址类型的[联系人](contact.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|String|联系人电子邮件地址。|
|name|String|联系人的显示名称。|
|type |字符串 |电子邮件地址类型。 可取值为：`unknown`、`work`、`personal`、`main`、`other`。 默认值是`unknown`，这意味着**地址**尚未设置为特定的类型。 |
|otherLabel |String  |若要指定自定义类型的电子邮件地址，请将**类型**设置为`other`，并将**otherLabel**分配给自定义字符串。 例如，您可以使用特定的电子邮件地址您自愿活动。 **类型**设置为`other`，如设置为自定义字符串**otherLabel** `Volunteer work`。 |

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
  "suppressions": [
    "Error: /api-reference/beta/resources/typedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
