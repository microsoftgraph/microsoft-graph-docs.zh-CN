---
title: expeditedQualityUpdateReference 资源类型
description: 表示Windows 10质量更新内容以加快更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 685f65d8c5661cd4c8308ed712ab3fddedbae51d
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067877"
---
# <a name="expeditedqualityupdatereference-resource-type"></a>expeditedQualityUpdateReference 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Windows 10质量更新内容以加快更新。

在部署中，相同的快速质量更新参考可能会导致设备接收不同的更新修订，但内容被视为与部署中所有设备的上下文等效。

继承自 [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|classification|microsoft.graph.windowsUpdates.qualityUpdateClassification|指定所引用内容的分类。 支持 **qualityUpdateClassification 值的子集**。 默认值为 `security`。 可能的值是 `security` ：。 继承自 [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md)。|
|equivalentContent|microsoft.graph.windowsUpdates.equivalentContentOption|指定要视为等效内容的其他内容。 支持 **equivalentContentOption 值的子集**。 默认值为 `latestSecurity`。 可能的值是 `latestSecurity` ：。|
|releaseDateTime|DateTimeOffset|按给定分类的发布日期指定质量更新 (即指定日期发布的最后一个) 。 任何具有在 **releaseDateTime** 之前发布的更新的设备都将收到快速的质量更新。 继承自 [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)",
  "equivalentContent": "String"
}
```

