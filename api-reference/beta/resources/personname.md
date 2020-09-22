---
title: Contact.personname 资源类型
description: Contact.personname 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1f1817e3d9868e47158453113f4781ebfc155f86
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997940"
---
# <a name="personname-resource-type"></a>Contact.personname 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表用户提供的、与其在 [配置文件](../resources/profile.md)中关联的扩展名称信息。

继承自 [itemFacet](../resources/itemfacet.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出名称](../api/profile-list-names.md)|[contact.personname](../resources/personname.md) 集合|从 "名称" 导航属性中获取 Contact.personname 资源。|
|[创建 Contact.personname](../api/profile-post-names.md)|[Contact.personname](../resources/personname.md)|从 "名称" 导航属性中创建一个新的 [contact.personname](../resources/personname.md) 对象。|
|[获取 Contact.personname](../api/personname-get.md)|[Contact.personname](../resources/personname.md)|读取 [contact.personname](../resources/personname.md) 对象的属性和关系。|
|[更新 Contact.personname](../api/personname-update.md)|[Contact.personname](../resources/personname.md)|更新 [contact.personname](../resources/personname.md) 对象的属性。|
|[删除 Contact.personname](../api/personname-delete.md)|无|删除一个 [contact.personname](../resources/personname.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|displayName|String|根据用户或其设备的区域设置，提供 firstName 和 lastName 的顺序呈现。|
|前|String|用户的名字。|
|id|String|用于单独寻址实体的标识符。 继承自 [entity](../resources/entity.md)|
|推导|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断的，则包含推理详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|initials|String|用户的首字母缩写。|
|languageTag|String|包含以下语言的名称： (en-us、无 NB、en-us) 以下 IETF BCP47 格式。   |
|末|String|用户的姓氏。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|maiden|String|Maiden 用户的名称。 |
|中间|String|用户的中间名。|
|昵称|String|用户的昵称。|
|拼音|[yomiPersonName](../resources/yomipersonname.md)|有关如何对用户名称进行发音的指南。|
|source|[personDataSource](../resources/persondatasource.md)|值的来源，如果从另一个服务同步。 继承自 [itemFacet](../resources/itemfacet.md)。|
|后缀|String|用户名称之后使用的指示符 (例如：博士. )   |
|title|String|Honorifics 用于为用户名称加上前缀 (例如： Dr.、罗德、Madam、Mrs ) |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personName",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personName",
  "id": "e13f7a4d-303c-464f-a6af-80ea18eb74f3",
  "allowedAudiences": "organization",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null,
  "middle": null,
  "nickname": "Kesha",
  "suffix": null,
  "title": null,
  "pronunciation": {
    "@odata.type": "microsoft.graph.yomiPersonName"
  }
}
```

