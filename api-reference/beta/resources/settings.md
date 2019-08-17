---
title: 设置资源类型
description: 用户使用分析 API 时所需的当前设置。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a7d534aecf6e7ffa427ea175ae06e2b1820435b2
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450728"
---
# <a name="settings-resource-type"></a>设置资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户使用分析 API 时所需的当前设置。

若要使分析 API 返回用户的结果, 他们必须拥有为 Microsoft Graph 启用的云托管邮箱, 具有有效的 MyAnalytics 许可证, 并选择使用 MyAnalytics。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
[获取设置](../api/useranalytics-get-settings.md) | [settings](settings.md) | 获取用户的以下属性设置。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hasGraphMailbox|Boolean|指定用户的主邮箱是否托管在云中, 是否已为 Microsoft Graph 启用。|
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