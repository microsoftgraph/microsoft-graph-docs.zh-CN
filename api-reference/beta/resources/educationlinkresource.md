---
title: educationLinkResource 资源类型
description: educationResource 的子类。 此资源是链接, 不具有与之关联的任何其他数据。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cd6e2d05fec5bebc00545947023a7ebc7c7150a1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334231"
---
# <a name="educationlinkresource-resource-type"></a>educationLinkResource 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationResource](educationresource.md)的子类。 此资源是链接, 不具有与之关联的任何其他数据。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|link|String|指向资源的 URL。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
