---
title: personWebsite 资源类型
description: 表示与各种服务中的用户关联的网站的详细信息。
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c26bda366fe03893e138551cb3ae3e8ab1efd8c8
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900469"
---
# <a name="personwebsite-resource-type"></a>personWebsite 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与各种服务中的用户关联的网站的详细信息。

继承自 [itemFacet](itemfacet.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出网站](../api/profile-list-websites.md)|[personWebsite](../resources/personwebsite.md) 集合|从网站导航属性获取 personWebsite 资源。|
|[创建 personWebsite](../api/profile-post-websites.md)|[personWebsite](../resources/personwebsite.md)|创建新的 personWebsite 对象。|
|[获取 personWebsite](../api/personwebsite-get.md)|[personWebsite](../resources/personwebsite.md)|读取 [personWebsite](../resources/personwebsite.md) 对象的属性和关系。|
|[更新 personWebsite](../api/personwebsite-update.md)|[personWebsite](../resources/personwebsite.md)|更新 [personWebsite](../resources/personwebsite.md) 对象的属性。|
|[删除 personWebsite](../api/personwebsite-delete.md)|无|删除 [personWebsite](../resources/personwebsite.md) 对象。|

## <a name="properties"></a>属性

| 属性     | 类型              | 说明                                                                                   |
|:-------------|:------------------|:----------------------------------------------------------------------------------------------|
|类别    |String collection  | 包含用户与网站关联的类别 (例如个人食谱) 。  |
|description   |字符串             | 包含网站的说明。                                                        |
|displayName   |字符串             | 包含网站的友好名称。                                                     |
|webUrl        |String             | 包含指向网站本身的链接。                                                        |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personWebsite",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "categories": [
    "String"
  ],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```


