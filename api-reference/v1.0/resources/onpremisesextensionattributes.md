---
title: onPremisesExtensionAttributes 资源类型
description: User 实体的 **onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性的属性。 对于 **onPremisesSyncEnabled** 用户，这组属性在本地 Active Directory 中使用并同步到 Azure AD，并且是只读的。 对于仅限云的用户 (其中 **onPremisesSyncEnabled** 为 false) ，可以在创建或更新期间设置这些属性。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 218bf0db4b615072ed3292311a26033279b1d803
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056434"
---
# <a name="onpremisesextensionattributes-resource-type"></a>onPremisesExtensionAttributes 资源类型

命名空间：microsoft.graph

[User](user.md)实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。 对于 **onPremisesSyncEnabled** 用户，此属性集的权威来源是同步到 Azure AD 的本地 Active Directory，并且是只读的。 对于仅限云的用户 (其中 **onPremisesSyncEnabled** 为 false) ，可以在创建或更新期间设置这些属性。

> **注意：** 这些扩展属性也称为 Exchange 自定义属性1-15。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|extensionAttribute1|String| 第一个可自定义的扩展属性。 |
|extensionAttribute2|String| 第二个可自定义扩展属性。 |
|extensionAttribute3|String| 第三个可自定义的扩展属性。 |
|extensionAttribute4|String| 第四个可自定义的扩展属性。 |
|extensionAttribute5|String| 第五个可自定义的扩展属性。 |
|extensionAttribute6|String| 第六个可自定义的扩展属性。 |
|extensionAttribute7|String| 第七个可自定义的扩展属性。 |
|extensionAttribute8|String| 第8个可自定义的扩展属性。 |
|extensionAttribute9|String| 第九个可自定义的扩展属性。 |
|extensionAttribute10|String| 第十个可自定义的扩展属性。 |
|extensionAttribute11|String| 第11个可自定义的扩展属性。 |
|extensionAttribute12|String| 第十二个可自定义的扩展属性。 |
|extensionAttribute13|String| 第十三个可自定义的扩展属性。 |
|extensionAttribute14|String| 第十四个可自定义的扩展属性。 |
|extensionAttribute15|String| 第十五个可自定义的扩展属性。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

