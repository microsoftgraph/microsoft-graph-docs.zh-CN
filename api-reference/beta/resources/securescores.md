---
title: secureScores 资源类型
description: '顶部 = n，其中 n = 要检索的数据的天数。 '
localization_priority: Normal
ms.openlocfilehash: fef5c43130aecf1604677d07f785a0cee0539568
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576078"
---
# <a name="securescores-resource-type"></a>secureScores 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表租户的租户和控制级别记分数据，每天安全分数。 默认情况下保留 90 天的数据。 此数据排序依据**createdDateTime**，从最新公开到最早。 这将允许您向页响应使用 $top = n，其中 n = 要检索的数据的天数。 


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |读取属性和 secureScores 对象的元数据。|


## <a name="properties"></a>属性
实体类型包含属性的租户安全得分 （每日快照数据）。

|属性 |类型 |说明 |
|:--|:--|:--|
|   azureTenantId   |   String  |   GUID string 租户 id。  |
|   createdDateTime |   DateTimeOffset  |   创建实体的日期。  |
|   id  |   String  |   AzureTenantId_createdDateTime 的组合。   |
|   licensedUserCount   |   Int32   |   许可的给定租户的用户计数。    |
|   activeUserCount |   Int32   |   给定租户的活动用户数。  |
|   currentScore    |   双精度  |   在指定日期的租户当前获得分数。    |
|   maxScore |  双精度  |   在指定日期租户最大得分。    |
|   enabledServices |   String 集合   |   租户 （例如，Exchange online、 Skype、 Sharepoint） 的 Microsoft 提供服务。   |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md)集合    |按不同的作用域 （例如，按行业，平均由安装的平均） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 范围内的平均得分。 |
|   controlScores | [controlScore](controlscore.md)集合  |   包含租户分数的一组控件。   |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) | 包含有关安全产品/服务供应商、 提供商和 subprovider 详细信息 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。|

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
    "azureTenantId": "String (identifier)",
    "createdDateTime": "DateTimeOffset",
    "licensedUserCount": "Int32",
    "activeUserCount": "Int32",
    "currentScore": "Double",
    "maxScore": "Double",    
    "enabledServices": ["String"],
    "averageComparativeScores": [{ "@odata.type":"microsoft.graph.averageComparativeScores"}],
    "controlScores": [{"@odata.type":"microsoft.graph.controlScores"}],
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
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
