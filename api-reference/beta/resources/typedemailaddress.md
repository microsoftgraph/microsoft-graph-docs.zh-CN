---
title: typedEmailAddress 资源类型
description: 表示联系人的姓名、电子邮件地址及其相应的电子邮件地址类型。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: mail
author: kevinbellinger
ms.openlocfilehash: 849e566919b22ddaa9c12a275f19139701bf467d
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66723487"
---
# <a name="typedemailaddress-resource-type"></a>typedEmailAddress 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [联系](contact.md)人的姓名、电子邮件地址及其相应的电子邮件地址类型。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|String|联系人的电子邮件地址。|
|name|String|联系人的显示名称。|
|type |字符串 |电子邮件地址的类型。 可取值为：`unknown`、`work`、`personal`、`main`、`other`。 默认值为 `unknown`，这意味着 **地址** 尚未设置为特定类型。 |
|otherLabel |String  |若要指定电子邮件地址的自定义类型，请将 **类型** 设置为 `other`，并将 **otherLabel** 分配给自定义字符串。 例如，可以为志愿者活动使用特定的电子邮件地址。 将 **类型** 设置为 `other`，并将 **otherLabel** 设置为自定义字符串，例如 `Volunteer work`。 |

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


