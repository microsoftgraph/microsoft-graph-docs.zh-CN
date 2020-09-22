---
title: companyDetail 资源类型
description: companyDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 93b5490048c149ca526a9c3d0024175c1c20d7e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033928"
---
# <a name="companydetail-resource-type"></a>companyDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与其 [配置文件](profile.md)中的实体相关的公司的信息。

## <a name="properties"></a>属性

| 属性       | 类型                                | 说明                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|address         |[physicalAddress](physicaladdress.md)| 公司的地址。                     |
|department      |String                               | 公司内的部门名称。           |
|displayName     |String                               | 公司名称。                               |
|officeLocation  |String                               | 所引用人员的办公室位置。  |
|拼音   |String                               | 公司名称的发音指南。   |
|WebUrl          |String                               | 链接到公司主页。              |

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

