---
title: companyDetail 资源类型
description: companyDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: dc8da38c9da8d6631e8e46199f420ae0b3ab652e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507581"
---
# <a name="companydetail-resource-type"></a>companyDetail 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与其[配置文件](profile.md)中的实体相关的公司的信息。

## <a name="properties"></a>属性

| 属性       | 类型                                | 说明                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|address         |[physicalAddress](physicaladdress.md)| 公司的地址。                     |
|department      |String                               | 公司内的部门名称。           |
|displayName     |String                               | 公司名称。                               |
|officeLocation  |String                               | 所引用人员的办公室位置。  |
|拼音   |String                               | 公司名称的发音指南。   |
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