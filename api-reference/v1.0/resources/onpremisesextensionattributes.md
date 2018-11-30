---
title: onPremisesExtensionAttributes 资源类型
description: 用户实体的**onPremisesExtensionAttributes**属性包含 15 个自定义扩展特性的属性。 此组属性是**onPremisesSyncEnabled**用户掌握了内部部署 Active Directory 中和同步到 Azure AD 和是只读的。 仅限云用户 （其中**onPremisesSyncEnabled**为 false），这些属性的创建过程中可以设置或更新。
ms.openlocfilehash: e5a56b5a846cf48cfc819b6d884689be10d6992e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009864"
---
# <a name="onpremisesextensionattributes-resource-type"></a>onPremisesExtensionAttributes 资源类型

[用户](user.md)实体的**onPremisesExtensionAttributes**属性包含 15 个自定义扩展特性的属性。 此组属性是**onPremisesSyncEnabled**用户掌握了内部部署 Active Directory 中和同步到 Azure AD 和是只读的。 仅限云用户 （其中**onPremisesSyncEnabled**为 false），这些属性的创建过程中可以设置或更新。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|extensionAttribute1|字符串| 第一个可自定义扩展属性。 |
|extensionAttribute2|字符串| 第二个可自定义扩展属性。 |
|extensionAttribute3|字符串| 第三个可自定义扩展属性。 |
|extensionAttribute4|字符串| 第四个可自定义扩展属性。 |
|extensionAttribute5|字符串| 第五个可自定义扩展属性。 |
|extensionAttribute6|字符串| 第六个可自定义扩展属性。 |
|extensionAttribute7|字符串| 第七个可自定义扩展属性。 |
|extensionAttribute8|字符串| 第八个可自定义扩展属性。 |
|extensionAttribute9|字符串| 第九个可自定义扩展属性。 |
|extensionAttribute10|字符串| 第十个可自定义扩展属性。 |
|extensionAttribute11|字符串| 第十一个可自定义扩展属性。 |
|extensionAttribute12|字符串| 第十二个可自定义扩展属性。 |
|extensionAttribute13|字符串| 第十三个可自定义扩展属性。 |
|extensionAttribute14|字符串| 第十四个可自定义扩展属性。 |
|extensionAttribute15|字符串| 第十五个可自定义扩展属性。 |

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