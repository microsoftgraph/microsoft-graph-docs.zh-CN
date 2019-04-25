---
title: secureScores 资源类型
description: 'top = n, 其中 n = 要检索的数据的天数。 '
localization_priority: Normal
ms.openlocfilehash: 8b4be9822b782303efe38dbdf5bd43e1ee543421
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549200"
---
# <a name="securescores-resource-type"></a>secureScores 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户和控制级别上的每日记分数据的租户安全分数。 默认情况下, 将保留90天的数据。 此数据按**createdDateTime**进行排序, 从最新到最早。 这将允许您使用 $top = n 对响应进行分页, 其中 n = 要检索的数据的天数。 


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |读取 secureScores 对象的属性和元数据。|


## <a name="properties"></a>属性
包含租户安全分数 (每日快照数据) 的属性的实体类型。

|属性 |类型 |说明 |
|:--|:--|:--|
|   azureTenantId   |   String  |   租户 ID 的 GUID 字符串。  |
|   createdDateTime |   DateTimeOffset  |   创建实体的日期。  |
|   id  |   String  |   azureTenantId_createdDateTime 的组合。   |
|   licensedUserCount   |   Int32   |   给定租户的许可用户计数。    |
|   activeUserCount |   Int32   |   给定租户的活动用户计数。  |
|   currentScore    |   双精度  |   租户当前在指定日期的得分。    |
|   maxScore |  双精度  |   指定日期上可能的租户最大分数。    |
|   enabledServices |   String collection   |   适用于租户的 Microsoft 提供的服务 (例如, Exchange online、Skype、Sharepoint)。   |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md)集合    |作用域内不同作用域 (例如, 按行业划分的平均分数、按座位的平均方式) 和控制类别 (标识、数据、设备、应用程序、基础结构)。 |
|   controlScores | [controlScore](controlscore.md)集合  |   包含一组控件的租户分数。   |


## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
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
}

```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescores.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
