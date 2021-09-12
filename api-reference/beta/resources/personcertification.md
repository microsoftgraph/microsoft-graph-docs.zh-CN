---
title: personCertification 资源类型
description: personCertification 资源类型
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ce360bd663549e7dc5fb0b9d9f1ccbce28f8dc15
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017098"
---
# <a name="personcertification-resource-type"></a>personCertification 资源类型

命名空间：microsoft.graph

表示已与用户配置文件关联的认证或 [指定](../resources/profile.md)。

继承自 [itemFacet](../resources/itemfacet.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出认证](../api/profile-list-certifications.md)|[personCertification](../resources/personcertification.md) 集合|从 certifications 导航属性获取 personCertification 资源。|
|[创建 personCertification](../api/profile-post-certifications.md)|[personCertification](../resources/personcertification.md)|创建新的 personCertification 对象。|
|[获取 personCertification](../api/personCertification-get.md)|[personCertification](../resources/personcertification.md)|读取 [personCertification 对象的属性和](../resources/personcertification.md) 关系。|
|[更新 personCertification](../api/personCertification-update.md)|[personCertification](../resources/personcertification.md)|更新 [personCertification 对象](../resources/personcertification.md) 的属性。|
|[删除 personCertification](../api/personCertification-delete.md)|None|删除 [personCertification](../resources/personcertification.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|certificationId  |String      |证书的可引用标识符。 |
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|说明      |String      |认证说明。                   |
|displayName      |String      |认证的标题。                         |
|endDate          |日期        |认证到期的日期。            |
|id|String|用于单独寻址实体的标识符。 继承自 [实体](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|issuedDate       |日期        |颁发证书的日期。         |
|issuingAuthority |String      |授予证书的颁发机构。          |
|issuingCompany   |String      |授予认证的公司。          |
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值源自何处。 继承自 [itemFacet](../resources/itemfacet.md)。|
|startDate        |日期        |认证生效的日期。       |
|thumbnailUrl     |String      |引用认证缩略图的 URL。   |
|WebUrl           |String      |引用证书的 URL。                  |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personCertification",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personCertification",
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
  "certificationId": "String",
  "description": "String",
  "displayName": "String",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "issuingCompany": "String",
  "startDate": "Date",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```


