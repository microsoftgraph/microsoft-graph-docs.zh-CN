---
title: expeditedQualityUpdateReference 资源类型
description: 表示Windows 10质量更新内容以加快更新。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: fa89e4c7cb8a20431b07b88e4d2eb92193d7148c
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861120"
---
# <a name="expeditedqualityupdatereference-resource-type"></a>expeditedQualityUpdateReference 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Windows 10质量更新内容以加快更新。

在部署中，相同的快速质量更新参考可能导致设备接收不同的更新修订，但内容被视为与部署中所有设备的上下文等效。

继承自 [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|classification|microsoft.graph.windowsUpdates.qualityUpdateClassification|指定所引用内容的分类。 支持 **qualityUpdateClassification 值的子集**。 默认值为 `security`。 可取值为：`security`、`unknownFutureValue`。 继承自 [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md)。|
|equivalentContent|microsoft.graph.windowsUpdates.equivalentContentOption|指定要视为等效内容的其他内容。 支持 **equivalentContentOption 值的子集**。 默认值为 `latestSecurity`。 可取值为：`latestSecurity`、`unknownFutureValue`。|
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

