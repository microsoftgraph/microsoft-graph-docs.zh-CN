---
title: educationalActivity 资源类型
description: educationalActivity 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 5f920b2afbb319af923212563aac6e8ea163c9de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055678"
---
# <a name="educationalactivity-resource-type"></a>educationalActivity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户已提供与 undergraduate、毕业、postgraduate 或其他教学活动相关的数据。

继承 [itemFacet](itemfacet.md)中的元数据属性。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 educationalActivities](../api/profile-list-educationalactivities.md)|[educationalActivity](../resources/educationalactivity.md) 集合|从 educationalActivities 导航属性中获取 educationalActivity 资源。|
|[创建 educationalActivity ](../api/profile-post-educationalactivities.md)|[educationalActivity](../resources/educationalactivity.md)|创建新的 educationalActivity 对象。|
|[获取 educationalActivity](../api/educationalactivity-get.md)|[educationalActivity](../resources/educationalactivity.md)|读取 [educationalActivity](../resources/educationalactivity.md) 对象的属性和关系。|
|[更新 educationalActivity](../api/educationalactivity-update.md)|[educationalActivity](../resources/educationalactivity.md)|更新 [educationalActivity](../resources/educationalactivity.md) 对象的属性。|
|[删除 educationalActivity](../api/educationalactivity-delete.md)|无|删除一个 [educationalActivity](../resources/educationalactivity.md) 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|completionMonthYear|日期|用户逐步或完成活动的月份和年份。 |
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|endMonthYear|日期|用户完成所引用的教育活动的月份和年份。|
|id|String|用于单独寻址实体的标识符。 继承自 [entity](../resources/entity.md)|
|推导|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断的，则包含推理详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|机构|[institutionData](../resources/institutiondata.md)|包含在上研究的机构的详细信息。 |
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|主程序|[educationalActivityDetail](../resources/educationalactivitydetail.md)|包含有关程序或课程的扩展信息。|
|source|[personDataSource](../resources/persondatasource.md)|值的来源，如果从另一个服务同步。 继承自 [itemFacet](../resources/itemfacet.md)。|
|startMonthYear|日期|用户 commenced 引用的活动的月份和年份。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationalActivity",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationalActivity",
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
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "@odata.type": "microsoft.graph.institutionData"
  },
  "program": {
    "@odata.type": "microsoft.graph.educationalActivityDetail"
  },
  "startMonthYear": "Date"
}
```

