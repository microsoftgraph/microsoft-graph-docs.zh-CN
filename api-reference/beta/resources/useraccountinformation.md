---
title: userAccountInformation 资源类型
description: userAccountInformation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 9bcd0553c51d75724f28737321f463bcab034306
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057911"
---
# <a name="useraccountinformation-resource-type"></a>userAccountInformation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表特定绑定到用户帐户的信息，无论是作为 Azure AD 帐户还是 Microsoft 帐户。 实体标识符分别设置为相应的 Azure AD guid 或 Microsoft 帐户 CID。 这些字段在 Microsoft Graph 中是只读的，并且必须通过用户配置文件或租户管理员在相应的体验上进行编辑。

继承自 [itemFacet](itemfacet.md)。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列表帐户](../api/profile-list-accounts.md)|[userAccountInformation](../resources/useraccountinformation.md) 集合|从帐户导航属性中获取 userAccountInformation 资源。|
|[创建 userAccountInformation](../api/profile-post-accounts.md)|[userAccountInformation](../resources/useraccountinformation.md)|创建新的 userAccountInformation 对象。|
|[获取 userAccountInformation](../api/useraccountinformation-get.md)|[userAccountInformation](../resources/useraccountinformation.md)|读取 [userAccountInformation](../resources/useraccountinformation.md) 对象的属性和关系。|
|[更新 userAccountInformation](../api/useraccountinformation-update.md)|[userAccountInformation](../resources/useraccountinformation.md)|更新 [userAccountInformation](../resources/useraccountinformation.md) 对象的属性。|
|[删除 userAccountInformation](../api/useraccountinformation-delete.md)|无|删除一个 [userAccountInformation](../resources/useraccountinformation.md) 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|ageGroup|String|显示用户的年龄组。 允许的 `null` 值 `minor` 、 `notAdult` 和 `adult` 由目录生成且不能更改。|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|countryCode|String|包含与用户帐户关联的双字符国家/地区代码。  |
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|id|String|用于单独寻址实体的标识符。 继承自 [entity](../resources/entity.md)|
|推导|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断的，则包含推理详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|preferredLanguageTag|[localeInfo](../resources/localeinfo.md)|包含用户与帐户相关的首选语言。   |
|source|[personDataSource](../resources/persondatasource.md)|值的来源，如果从另一个服务同步。 继承自 [itemFacet](../resources/itemfacet.md)。|
|userPrincipalName|String|与帐户关联的用户的用户主体名称 (UPN) 。   |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAccountInformation",
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
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "userPrincipalName": "String"
}
```


