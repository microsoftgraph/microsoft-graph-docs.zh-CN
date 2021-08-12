---
title: secureScore 资源类型
description: 表示租户和控制级别的租户每天评分数据的安全分数。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fbc942784813545f5d276addbd4581cf30ea82c8c2d8d6cf17d5f3ef3fbc7246
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180479"
---
# <a name="securescore-resource-type"></a>secureScore 资源类型

命名空间：microsoft.graph

表示租户和控制级别的租户每天评分数据的安全分数。 默认情况下，将存储 90 天的数据。 此数据按 **createdDateTime** 排序，从最新到最早。 这将允许您使用 $top=n 对响应进行页面响应，其中 n = 要检索的数据的天数。 


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
|   createdDateTime |   DateTimeOffset  |   实体的创建日期。  |
|   currentScore    |   双精度  |   指定日期的租户当前获得分数。    |
|   enabledServices |   String collection   |   Microsoft 为租户租户提供的服务 (例如，Exchange、Skype、Sharepoint) 。   |
|   licensedUserCount   |   Int32   |   给定租户的许可用户计数。    |
|   maxScore |  双精度  |   指定日期的租户最大可能分数。    |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md) 集合    |按不同范围的分数 (例如，按行业平均值、按) 和控件类别 (标识、数据、设备、应用、基础结构) 范围内的平均分数。 |
|   controlScores | [controlScore](controlscore.md) 集合  |   包含一组控件的租户分数。   |
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|复杂类型，包含有关安全产品/服务供应商、提供程序和子 (的详细信息，例如，vendor=Microsoft;provider=SecureScore) 。 必填。|


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

