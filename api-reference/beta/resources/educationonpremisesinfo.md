---
title: educationOnPremisesInfo 资源类型
description: 用于将本地 Active Directory 用户帐户与 Azure AD 用户对象相关联的其他信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c147755aea584674e17f2de913e039b7d3e0cf82
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764741"
---
# <a name="educationonpremisesinfo-resource-type"></a>educationOnPremisesInfo 资源类型

用于将本地 Active Directory 用户帐户与 Azure AD 用户对象相关联的其他信息。

## <a name="properties"></a>属性

| 属性    | 类型   | 说明                                               |
| :---------- | :----- | :-------------------------------------------------------- |
| immutableId | String | Active Directory 中的 user 对象的唯一标识符。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}-->

```json
{
  "immutableId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOnPremisesInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
