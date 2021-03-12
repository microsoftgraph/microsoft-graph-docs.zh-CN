---
title: onPremisesExtensionAttributes 资源类型
description: user **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。 对于 **onPremisesSyncEnabled** 用户，这组属性在本地 Active Directory 中托管并同步到 Azure AD，并且为只读。 对于仅云用户 (**onPremisesSyncEnabled** 为 false) ，可以在创建或更新期间设置这些属性。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c8e44879b3248cab502ee2aeabdaa732a2b35e1f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718955"
---
# <a name="onpremisesextensionattributes-resource-type"></a>onPremisesExtensionAttributes 资源类型

命名空间：microsoft.graph

user **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。 [](user.md) 对于 **onPremisesSyncEnabled** 用户，这组属性的颁发机构是同步到 Azure AD 且只读的本地 Active Directory。 对于仅云用户 (**onPremisesSyncEnabled** 为 false) ，可以在创建或更新期间设置这些属性。

> **注意：** 这些扩展属性也称为 Exchange 自定义属性 1-15。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|extensionAttribute1|字符串| 第一个可自定义的扩展属性。 |
|extensionAttribute2|字符串| 第二个可自定义的扩展属性。 |
|extensionAttribute3|字符串| 第三个可自定义的扩展属性。 |
|extensionAttribute4|字符串| 第四个可自定义的扩展属性。 |
|extensionAttribute5|字符串| 第五个可自定义的扩展属性。 |
|extensionAttribute6|字符串| 第六个可自定义的扩展属性。 |
|extensionAttribute7|字符串| 第七个可自定义的扩展属性。 |
|extensionAttribute8|字符串| 第八个可自定义的扩展属性。 |
|extensionAttribute9|字符串| 第九个可自定义的扩展属性。 |
|extensionAttribute10|字符串| 第十个可自定义的扩展属性。 |
|extensionAttribute11|字符串| 第十一个可自定义的扩展属性。 |
|extensionAttribute12|字符串| 第十二个可自定义的扩展属性。 |
|extensionAttribute13|字符串| 第十三个可自定义的扩展属性。 |
|extensionAttribute14|字符串| 第十四个可自定义的扩展属性。 |
|extensionAttribute15|字符串| 第十五个可自定义的扩展属性。 |

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

