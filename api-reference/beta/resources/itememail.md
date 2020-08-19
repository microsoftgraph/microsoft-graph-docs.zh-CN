---
title: itemEmail 资源类型
description: itemEmail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0a8a69ae484afab6b558890fbd186a4850235ead
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809425"
---
# <a name="itememail-resource-type"></a>itemEmail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与用户相关联的电子邮件地址的详细信息。

继承自 [itemFacet](../resources/itemfacet.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出电子邮件](../api/profile-list-emails.md)|[itemEmail](../resources/itememail.md) 集合|从 "电子邮件" 导航属性中获取 itemEmail 资源。|
|[创建 itemEmail](../api/profile-post-emails.md)|[itemEmail](../resources/itememail.md)|创建新的 itemEmail 对象。|
|[获取 itemEmail](../api/itememail-get.md)|[itemEmail](../resources/itememail.md)|读取 [itemEmail](../resources/itememail.md) 对象的属性和关系。|
|[更新 itemEmail](../api/itememail-update.md)|[itemEmail](../resources/itememail.md)|更新 [itemEmail](../resources/itememail.md) 对象的属性。|
|[删除 itemEmail](../api/itememail-delete.md)|无|删除一个 [itemEmail](../resources/itememail.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|address|String|电子邮件地址本身。|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|displayName|String|用户与特定电子邮件地址相关联的名称或标签。|
|id|String|用于单独寻址实体的标识符。 继承自 [entity](../resources/entity.md)|
|推导|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断的，则包含推理详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|source|[personDataSource](../resources/persondatasource.md)|值的来源，如果从另一个服务同步。 继承自 [itemFacet](../resources/itemfacet.md)。|
|type|emailType|电子邮件地址的类型。 可取值为：`unknown`、`work`、`personal`、`main`、`other`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemEmail",
  "id": "0f30bf5d-bf5d-0f30-5dbf-300f5dbf300f",
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
  "address": "String",
  "displayName": "String",
  "type": "String"
}
```
