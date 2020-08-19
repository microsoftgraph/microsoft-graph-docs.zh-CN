---
title: itemPatent 资源类型
description: itemPatent 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4b8a5c72117e20a73fb3c3b6b8a2af308219b69d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809636"
---
# <a name="itempatent-resource-type"></a>itemPatent 资源类型
 
命名空间：microsoft.graph

代表已添加到用户 [配置文件](../resources/profile.md)中的已授权或已存档的专利。

继承自 [itemFacet](../resources/itemfacet.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出专利](../api/profile-list-patents.md)|[itemPatent](../resources/itempatent.md) 集合|从专利导航属性中获取 itemPatent 资源。|
|[创建 itemPatent](../api/profile-post-patents.md)|[itemPatent](../resources/itempatent.md)|创建新的 itemPatent 对象。|
|[获取 itemPatent](../api/itempatent-get.md)|[itemPatent](../resources/itempatent.md)|读取 [itemPatent](../resources/itempatent.md) 对象的属性和关系。|
|[更新 itemPatent](../api/itempatent-update.md)|[itemPatent](../resources/itempatent.md)|更新 [itemPatent](../resources/itempatent.md) 对象的属性。|
|[删除 itemPatent](../api/itempatent-delete.md)|无|删除一个 [itemPatent](../resources/itempatent.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|description|String|专利或档案的 Descpription。 |
|displayName|String|专利或档案的标题。 |
|id|String|用于单独寻址实体的标识符。 继承自 [entity](../resources/entity.md)|
|推导|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断的，则包含推理详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|isPending        |布尔值     |指示专利处于待处理状态。        |
|issuedDate       |日期        |授予专利的日期。   |
|issuingAuthority |String      |授予专利的证书颁发机构。     |
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|数字           |String      |专利号码。                      |
|source|[personDataSource](../resources/persondatasource.md)|值的来源，如果从另一个服务同步。 继承自 [itemFacet](../resources/itemfacet.md)。|
|webUrl           |String      |引用专利或档案的 URL。 |


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPatent",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemPatent",
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
  "description": "String",
  "displayName": "String",
  "isPending": "Boolean",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "number": "String",
  "webUrl": "String"
}
```
