---
title: userAnalytics 资源类型
description: 用户的设置和活动统计信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ffe6830088bd60c4de9cea8def8e8202d1b33f13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519538"
---
# <a name="useranalytics-resource-type"></a>userAnalytics 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户的设置和活动统计信息。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
[获取设置](../api/useranalytics-get-settings.md) | [设置](settings.md) | 获取用户使用分析 API 的设置。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|设置|[设置](settings.md)|用户使用分析 API 的当前设置。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|activityStatistics|[activityStatistics](activitystatistics.md)集合| 用户在工作时间和工作时间之外花费时间的工作活动的集合。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [
    "activityStatistics"
  ],
  "@odata.type": "microsoft.graph.userAnalytics"
}-->

```json
{
  "id": "string",
  "settings": {"@odata.type": "microsoft.graph.settings"},
  "activityStatistics": [{"@odata.type": "microsoft.graph.activityStatistics"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAnalytics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
