---
title: secureScore 资源类型
description: 表示租户在租户和控制级别每天评分数据的安全分数。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 4773436fa1ef3f2e2465b99cd9c29e2d844d8b54
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900385"
---
# <a name="securescore-resource-type"></a>secureScore 资源类型

命名空间：microsoft.graph

表示租户在租户和控制级别每天评分数据的安全分数。 默认情况下，将保存 90 天的数据。 此数据按 **createdDateTime** 排序，从最新到最早。 这将允许你使用$top=n 对响应进行页面处理，其中 n = 要检索的数据天数。 


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScores](../api/security-list-securescores.md) | [secureScores](securescore.md) 集合 |获取 secureScore 对象集合。|
|[获取 secureScore](../api/securescore-get.md) | [secureScore](securescore.md) |读取 secureScore 对象的属性和元数据。 | 



## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|id |String|提供程序生成的 GUID/唯一标识符。 只读。 必填。|
|   azureTenantId   |   字符串  |   租户 ID 的 GUID 字符串。  |
|   activeUserCount |   Int32   |   给定租户的活动用户计数。  |
|   createdDateTime |   DateTimeOffset  |   创建实体的日期。  |
|   currentScore    |   双精度  |   租户当前在指定日期达到的分数。    |
|   enabledServices |   String collection   |   Microsoft 为租户 (提供的服务，例如 Exchange Online、Skype、Sharepoint) 。   |
|   licensedUserCount   |   Int32   |   给定租户的许可用户计数。    |
|   maxScore |  双精度  |   指定日期的租户最大可能分数。    |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md) 集合    |按不同范围 (的平均分数，例如，按行业划分的平均分数，按座位) 的平均分数，以及范围内的标识、数据、设备、应用、基础结构)  (控制类别的平均分数。 |
|   controlScores | [controlScore](controlscore.md) 集合  |   包含一组控件的租户分数。   |
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|复杂类型，包含有关安全产品/服务供应商、提供程序和子保护程序 (的详细信息，例如，供应商=Microsoft;provider=SecureScore) 。 必填。|


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
"id": "String (identifier)",
"azureTenantId": "String",
"activeUserCount": "Int32",
"createdDateTime": "String (timestamp)",
"currentScore": "Double",
"enabledServices": ["String"],
"licensedUserCount": "Int32",
"maxScore": "Double",
"averageComparativeScores": [{"@odata.type": "microsoft.graph.averageComparativeScore"}],
"controlScores": [{"@odata.type": "microsoft.graph.controlScore"}],
"vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

