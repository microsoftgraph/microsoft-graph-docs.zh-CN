---
title: conditionalAccessPlatforms 资源类型
description: 策略作用域中包含和排除的平台。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8ca88fb9fed1897659e1b6c126a22444ca652963f29bc2b208d3a259e386eabe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202516"
---
# <a name="conditionalaccessplatforms-resource-type"></a>conditionalAccessPlatforms 资源类型

命名空间：microsoft.graph

策略作用域中包含和排除的平台。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|includePlatforms|conditionalAccessDevicePlatform 集合| 可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`all` 或 `unknownFutureValue`。|
|excludePlatforms|conditionalAccessDevicePlatform 集合| 可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`all`、`unknownFutureValue`。|

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

