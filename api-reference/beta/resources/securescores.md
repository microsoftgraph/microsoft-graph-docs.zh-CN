---
title: secureScore 资源类型
description: 'top=n，其中 n = 要检索的数据天数。 '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 9565a507eac6d5c1be272749a45c6e4b234d5da2
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094093"
---
# <a name="securescore-resource-type"></a>secureScore 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户在租户和控制级别每天评分数据的安全分数。 默认情况下，将保存 90 天的数据。 此数据按 **createdDateTime** 排序，从最新到最早。 这将允许你使用$top=n 对响应进行页面处理，其中 n = 要检索的数据天数。


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |读取 secureScores 对象的属性和元数据。|


## <a name="properties"></a>属性
包含租户安全分数属性的实体类型 (每日快照数据) 。

|属性 |类型 |说明 |
|:--|:--|:--|
|   activeUserCount |   Int32   |   给定租户的活动用户计数。  |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md) 集合    |按不同范围 (的平均分数，例如，按行业划分的平均分数，按座位) 的平均分数，以及范围内的标识、数据、设备、应用、基础结构)  (控制类别的平均分数。 |
|   azureTenantId   |   字符串  |   租户 ID 的 GUID 字符串。  |
|   controlScores | [controlScore](controlscore.md) 集合  |   包含一组控件的租户分数。   |
|   createdDateTime |   DateTimeOffset  |   创建实体的日期。  |
|   currentScore    |   双精度  |   租户当前在指定日期达到的分数。    |
|   enabledServices |   字符串集合   |   Microsoft 为租户 (提供的服务，例如联机Exchange、Skype、SharePoint) 。   |
|   id  |   String  |   azureTenantId_createdDateTime的组合。   |
|   licensedUserCount   |   Int32   |   给定租户的许可用户计数。    |
|   maxScore |  双精度  |   指定日期的租户最大可能分数。    |




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
  "activeUserCount": "Int32",
  "averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
  "averageScore": "Double",
  "azureTenantId": "Guid",
  "controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
  "createdDate": "DateTimeOffset",
  "createdDateTime": "2019-02-07T20:33:53.156Z",
  "currentScore": "Int32",
  "enabledServices": "Collection(string)",
  "id": "String",
  "licensedUserCount": "Int32",
  "maxScore": "Int32"
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


