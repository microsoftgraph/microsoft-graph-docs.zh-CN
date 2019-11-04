---
title: companyDetail 资源类型
description: companyDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 04e33c9fdae1eae811ee88e7cdef95b4b97b2c3f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936837"
---
# <a name="companydetail-resource-type"></a>companyDetail 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与其[配置文件](profile.md)中的实体相关的公司的信息。

## <a name="properties"></a>属性

| 属性       | 类型                                | 说明                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|address         |[physicalAddress](physicaladdress.md)| 公司的地址。                     |
|department      |字符串                               | 公司内的部门名称。           |
|displayName     |String                               | 公司名称。                               |
|officeLocation  |字符串                               | 所引用人员的办公室位置。  |
|拼音   |字符串                               | 公司名称的发音指南。   |
|webUrl          |String                               | 链接到公司主页。              |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.companyDetail",
  "baseType": null
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "department": "String",
  "displayName": "String",
  "officeLocation": "String",
  "pronunciation": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "companyDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->