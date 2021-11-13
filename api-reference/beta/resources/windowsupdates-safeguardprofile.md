---
title: safeguardProfile 资源类型
description: 介绍 () 保护设备时所针对的问题。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 8c528111af41ee3340a58402f66d2e4ac5410aca
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890120"
---
# <a name="safeguardprofile-resource-type"></a>safeguardProfile 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍 () 保护设备时所针对的问题。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|category|microsoft.graph.windowsUpdates.safeguardCategory|指定安全措施的类别。 可能的值是 `likelyIssues` `unknownFutureValue` ：、。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.safeguardProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.safeguardProfile",
  "category": "String"
}
```

