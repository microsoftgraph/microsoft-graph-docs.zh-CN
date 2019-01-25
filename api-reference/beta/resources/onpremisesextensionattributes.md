---
title: onPremisesExtensionAttributes 资源类型
description: 用户实体的**onPremisesExtensionAttributes**属性包含 15 个自定义扩展特性的属性。 对于 onPremisesSyncEnabled 用户，此组属性在本地 Active Directory 中进行管理，并同步到 Azure AD，且为只读。 对于只使用云的用户（其中 onPremisesSyncEnabled 为 false），可以在创建或更新期间设置这些属性。
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518238"
---
# <a name="onpremisesextensionattributes-resource-type"></a>onPremisesExtensionAttributes 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[用户](user.md)实体的**onPremisesExtensionAttributes**属性包含 15 个自定义扩展特性的属性。 对于 onPremisesSyncEnabled 用户，此组属性在本地 Active Directory 中进行管理，并同步到 Azure AD，且为只读。 对于只使用云的用户（其中 onPremisesSyncEnabled 为 false），可以在创建或更新期间设置这些属性。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|extensionAttribute1|String| 第一个可自定义扩展属性。 |
|extensionAttribute2|String| 第二个可自定义扩展属性。 |
|extensionAttribute3|String| 第三个可自定义扩展属性。 |
|extensionAttribute4|String| 第四个可自定义扩展属性。 |
|extensionAttribute5|String| 第五个可自定义扩展属性。 |
|extensionAttribute6|String| 第六个可自定义扩展属性。 |
|extensionAttribute7|String| 第七个可自定义扩展属性。 |
|extensionAttribute8|String| 第八个可自定义扩展属性。 |
|extensionAttribute9|String| 第九个可自定义扩展属性。 |
|extensionAttribute10|String| 第十个可自定义扩展属性。 |
|extensionAttribute11|String| 第十一个可自定义扩展属性。 |
|extensionAttribute12|String| 第十二个可自定义扩展属性。 |
|extensionAttribute13|String| 第十三个可自定义扩展属性。 |
|extensionAttribute14|String| 第十四个可自定义扩展属性。 |
|extensionAttribute15|String| 第十五个可自定义扩展属性。 |

## <a name="json-representation"></a>JSON 表示形式

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesextensionattributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
