---
title: conditionalAccessPlatforms 资源类型
description: 策略作用域中包含和排除的平台。
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5dec75019dc01b4d1ec12b55b66c34f03cb53630
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804099"
---
# <a name="conditionalaccessplatforms-resource-type"></a>conditionalAccessPlatforms 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

策略作用域中包含和排除的平台。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|includePlatforms|conditionalAccessDevicePlatform 集合| 可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`all`、`unknownFutureValue`、`linux`。 请注意，必须使用此可 `Prefer: include-unknown-enum-members` 变化枚举 (请求) 获取以下 [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)： `linux`。 |
|excludePlatforms|conditionalAccessDevicePlatform 集合| 可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`all`、`unknownFutureValue`、`linux`。 请注意，必须使用此可 `Prefer: include-unknown-enum-members` 变化枚举 (请求) 获取以下 [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)： `linux`。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPlatforms",
  "baseType": null
}-->

```json
{
  "includePlatforms": ["String"],
  "excludePlatforms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPlatforms resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

