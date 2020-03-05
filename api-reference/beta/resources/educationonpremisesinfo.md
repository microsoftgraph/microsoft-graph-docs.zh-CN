---
title: educationOnPremisesInfo 资源类型
description: 用于将本地 Active Directory 用户帐户与 Azure AD 用户对象相关联的其他信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6695f1cd92ccde1fb26a581fce49c0c233deb141
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501512"
---
# <a name="educationonpremisesinfo-resource-type"></a>educationOnPremisesInfo 资源类型

命名空间： microsoft. graph

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
