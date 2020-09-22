---
title: 设置资源类型
description: 用户使用分析 API 时所需的当前设置。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 822ac02be4f3dc5d507aa5d9dbbb2fa22b194b64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033533"
---
# <a name="settings-resource-type"></a>设置资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户使用分析 API 时所需的当前设置。

若要使分析 API 返回用户的结果，他们必须拥有为 Microsoft Graph 启用的云托管邮箱，具有有效的 MyAnalytics 许可证，并选择使用 MyAnalytics。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
[获取设置](../api/useranalytics-get-settings.md) | [设置](settings.md) | 获取用户的以下属性设置。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hasGraphMailbox|Boolean|指定用户的主邮箱是否托管在云中，是否已为 Microsoft Graph 启用。|
|hasLicense|Boolean|指定是否为用户分配了 MyAnalytics 许可证。|
|hasOptedOut|Boolean|指定用户是否选择了 "MyAnalytics"。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settings",
  "baseType": null
}-->

```json
{
  "hasGraphMailbox": true,
  "hasLicense": true,
  "hasOptedOut": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

