---
title: qualityUpdateReference 资源类型
description: 表示Windows 10更新内容。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ecfddf24b8e2550f55c28ef60e218b5caae985da
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861596"
---
# <a name="qualityupdatereference-resource-type"></a>qualityUpdateReference 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Windows 10更新内容。

在部署中，相同的质量更新参考可能会导致设备接收不同的更新修订，但内容被视为与部署中所有设备的上下文等效。

继承自 [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md)。 [expeditedQualityUpdateReference 的基本类型](../resources/windowsupdates-expeditedqualityupdatereference.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|classification|microsoft.graph.windowsUpdates.qualityUpdateClassification|指定所引用内容的分类。 支持 **qualityUpdateClassification 值的子集**。 可取值为：`security`、`unknownFutureValue`。|
|releaseDateTime|DateTimeOffset|指定给定 servicingChannel 中的质量更新，按日期 (给定分类，即指定日期发布) 。 默认值为 `security`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)"
}
```

