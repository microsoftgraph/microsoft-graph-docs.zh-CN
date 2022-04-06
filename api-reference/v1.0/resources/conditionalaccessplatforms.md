---
title: conditionalAccessPlatforms 资源类型
description: 策略作用域中包含和排除的平台。
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ca34f949e910907910a2aa14e64951538ab4bb13
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672537"
---
# <a name="conditionalaccessplatforms-resource-type"></a>conditionalAccessPlatforms 资源类型

命名空间：microsoft.graph

策略作用域中包含和排除的平台。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|includePlatforms|conditionalAccessDevicePlatform 集合| 可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`linux`、`all`、`unknownFutureValue`。|
|excludePlatforms|conditionalAccessDevicePlatform 集合| 可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`linux`、`all`、`unknownFutureValue`。|

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

