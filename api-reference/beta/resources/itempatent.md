---
title: itemPatent 资源类型
description: itemPatent 资源类型
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a6e53816f9e239de0f1c928763d1e329cc8cb63f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063620"
---
# <a name="itempatent-resource-type"></a>itemPatent 资源类型
 
命名空间：microsoft.graph

表示已授予或已存档的已添加到用户配置文件的 [专利](../resources/profile.md)。

继承自 [itemFacet](../resources/itemfacet.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出专利](../api/profile-list-patents.md)|[itemPatent](../resources/itempatent.md) 集合|从专利导航属性获取 itemPatent 资源。|
|[创建 itemPatent](../api/profile-post-patents.md)|[itemPatent](../resources/itempatent.md)|创建新的 itemPatent 对象。|
|[获取 itemPatent](../api/itempatent-get.md)|[itemPatent](../resources/itempatent.md)|读取 [itemPatent](../resources/itempatent.md) 对象的属性和关系。|
|[更新 itemPatent](../api/itempatent-update.md)|[itemPatent](../resources/itempatent.md)|更新 [itemPatent 对象](../resources/itempatent.md) 的属性。|
|[删除 itemPatent](../api/itempatent-delete.md)|无|删除 [itemPatent](../resources/itempatent.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|说明|String|专利或归档的去向。 |
|displayName|String|专利或归档的标题。 |
|id|String|用于单独寻址实体的标识符。 继承自 [实体](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|isPending        |Boolean     |指示正在申请专利。        |
|issuedDate       |日期        |授予专利的日期。   |
|issuingAuthority |String      |授予专利的颁发机构。     |
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|数字           |String      |专利号。                      |
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值源自何处。 继承自 [itemFacet](../resources/itemfacet.md)。|
|WebUrl           |String      |引用专利或归档的 URL。 |


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


