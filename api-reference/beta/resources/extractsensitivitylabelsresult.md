---
title: extractSensitivityLabelsResult 资源类型
description: 表示 extractSensitivityLabels API 的响应格式。
author: jaLuthra
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a3533cecf651c6b98deb81b01cf06d5a08f2dc36
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917841"
---
# <a name="extractsensitivitylabelsresult-resource-type"></a>extractSensitivityLabelsResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [extractSensitivityLabels](../api/driveitem-extractsensitivitylabels.md) API 的响应格式。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|标签|[sensitivityLabelAssignment](./sensitivitylabelassignment.md) 集合|分配给文件的敏感度标签列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extractSensitivityLabelsResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extractSensitivityLabelsResult",
  "labels": [
    {
      "@odata.type": "microsoft.graph.sensitivityLabelAssignment"
    }
  ]
}
```

