---
title: itemFacet 资源类型
description: itemFacet 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ff186b8b78e0070b5f92efa1858ef8d15d51c59f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021432"
---
# <a name="itemfacet-resource-type"></a>itemFacet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [配置文件](profile.md) entityset 中的所有资源类型继承自的抽象基类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|allowedAudiences|能够查看关联实体内包含的值的访问群体。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。|
|createdDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。|
|id|String|用于单独寻址实体的标识符。 继承自 [entity](../resources/entity.md)|
|推导|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断的，则包含推理详细信息。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。|
|lastModifiedDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。|
|source|[personDataSource](../resources/persondatasource.md)|实体中的值的起源（如果从另一个服务同步）。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemFacet",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemFacet",
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
  }
}
```



