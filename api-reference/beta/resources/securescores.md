---
title: secureScore 资源类型
description: 'top = n，其中 n = 要检索的数据的天数。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 3db31203f9c5827459ab2149efbd3adb28030d0a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087542"
---
# <a name="securescore-resource-type"></a>secureScore 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户和控制级别上的每日记分数据的租户安全分数。 默认情况下，将保留90天的数据。 此数据按 **createdDateTime**进行排序，从最新到最早。 这将允许您使用 $top = n 对响应进行分页，其中 n = 要检索的数据的天数。


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScore](../api/securescores-list.md) | [secureScores](securescores.md) |读取 secureScores 对象的属性和元数据。|


## <a name="properties"></a>属性
包含租户安全分数的属性的实体类型 (每日快照数据) 。

|属性 |类型 |说明 |
|:--|:--|:--|
|   azureTenantId   |   字符串  |   租户 ID 的 GUID 字符串。  |
|   createdDateTime |   DateTimeOffset  |   创建实体的日期。  |
|   id  |   字符串  |   AzureTenantId_createdDateTime 的组合。   |
|   licensedUserCount   |   Int32   |   给定租户的许可用户计数。    |
|   activeUserCount |   Int32   |   给定租户的活动用户计数。  |
|   currentScore    |   双精度  |   租户当前在指定日期的得分。    |
|   maxScore |  双精度  |   指定日期上可能的租户最大分数。    |
|   enabledServices |   字符串集合   |   Microsoft 为租户提供的服务 (例如，Exchange online、Skype、Sharepoint) 。   |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md) 集合    |不同作用域的平均分数 (例如，行业平均值、座位) 和控制类别的平均 (标识、数据、设备、应用程序、基础结构) 在范围内。 |
|   controlScores | [controlScore](controlscore.md) 集合  |   包含一组控件的租户分数。   |


## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
  "id": "String",
  "azureTenantId": "Guid",
  "createdDate": "DateTimeOffset",
  "licensedUserCount": "Int32",
  "activeUserCount": "Int32",
  "currentScore": "Int32",
  "maxScore": "Int32",
  "averageScore": "Double",
  "enabledServices": "Collection(string)",
  "averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
  "controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
  "createdDateTime": "2019-02-07T20:33:53.156Z"
}

```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


