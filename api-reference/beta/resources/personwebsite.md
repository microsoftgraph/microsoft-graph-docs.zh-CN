---
title: personWebsite 资源类型
description: personWebsite 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: cf4386cf70179715880a1ae07db3dfbb5f07c224
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521895"
---
# <a name="personwebsite-resource-type"></a>personWebsite 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与各种服务中的用户相关联的网站的详细信息。

继承自[itemFacet](itemfacet.md)。

## <a name="methods"></a>方法

| 方法                                           | 返回类型                       | 说明                                                |
|:-------------------------------------------------|:----------------------------------|:-----------------------------------------------------------|
| [获取 personWebsite](../api/personwebsite-get.md) | [personWebsite](personwebsite.md) | 读取**personWebsite**对象的属性和关系。 |
| [更新 personWebsite](../api/personwebsite-update.md)         | [personWebsite](personwebsite.md) | 更新**personWebsite**对象。                               |
| [删除 personWebsite](../api/personwebsite-delete.md)         | 无                              | 删除**personWebsite**对象。                               |

## <a name="properties"></a>属性

| 属性     | 类型              | 说明                                                                         |
|:-------------|:------------------|:------------------------------------------------------------------------------------|
|categories    |String 集合  | 包含用户与网站相关联的类别（例如，个人、食谱）。  |
|说明   |字符串             | 包含网站的说明。                                              |
|displayName   |String             | 包含网站的友好名称。                                           |
|webUrl        |String             | 包含指向网站本身的链接。                                              |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personWebsite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
