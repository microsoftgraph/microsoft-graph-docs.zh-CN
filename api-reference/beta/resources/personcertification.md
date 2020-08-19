---
title: personCertification 资源类型
description: personCertification 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ef4ebe3bc870bafd0edf6a5315589c8f823286df
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812925"
---
# <a name="personcertification-resource-type"></a>personCertification 资源类型

命名空间：microsoft.graph

表示已与用户的 [配置文件](../resources/profile.md)关联的证书或称号。

继承自 [itemFacet](../resources/itemfacet.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出证书](../api/profile-list-certifications.md)|[personCertification](../resources/personcertification.md) 集合|从认证导航属性中获取 personCertification 资源。|
|[创建 personCertification](../api/profile-post-certifications.md)|[personCertification](../resources/personcertification.md)|创建新的 personCertification 对象。|
|[获取 personCertification](../api/personCertification-get.md)|[personCertification](../resources/personcertification.md)|读取 [personCertification](../resources/personcertification.md) 对象的属性和关系。|
|[更新 personCertification](../api/personCertification-update.md)|[personCertification](../resources/personcertification.md)|更新 [personCertification](../resources/personcertification.md) 对象的属性。|
|[删除 personCertification](../api/personCertification-delete.md)|无|删除一个 [personCertification](../resources/personcertification.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|certificationId  |String      |证书的 referenceable 标识符。 |
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|description      |String      |证书的说明。                   |
|displayName      |String      |证书的标题。                         |
|endDate          |日期        |证书到期的日期。            |
|id|String|用于单独寻址实体的标识符。 继承自 [entity](../resources/entity.md)|
|推导|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断的，则包含推理详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|issuedDate       |日期        |颁发证书的日期。         |
|issuingAuthority |String      |授予证书颁发机构的权限。          |
|issuingCompany   |String      |授予证书的公司。          |
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|source|[personDataSource](../resources/persondatasource.md)|值的来源，如果从另一个服务同步。 继承自 [itemFacet](../resources/itemfacet.md)。|
|startDate        |日期        |证书生效的日期。       |
|thumbnailUrl     |String      |URL 引用证书的缩略图。   |
|webUrl           |String      |引用证书的 URL。                  |

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
