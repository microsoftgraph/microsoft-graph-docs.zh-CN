---
title: monitoringSettings 资源类型
description: 设置控制部署中的自动监视和响应。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: aff5fa9571628783521dcc5ae0113e767915c2c7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067854"
---
# <a name="monitoringsettings-resource-type"></a>monitoringSettings 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置控制部署中的自动监视和响应。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|monitoringRules|[microsoft.graph.windowsUpdates.monitoringRule](../resources/windowsupdates-monitoringrule.md) 集合|指定监视信号触发对部署的操作时可通过的规则。 使用"or"组合规则。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringSettings",
  "monitoringRules": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
    }
  ]
}
```

