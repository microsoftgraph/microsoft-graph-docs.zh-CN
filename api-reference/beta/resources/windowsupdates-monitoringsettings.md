---
title: monitoringSettings 资源类型
description: 设置在部署中控制自动监视和响应。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: c00f7e714b68595ce1debbf155ec802f0f579f23
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61810435"
---
# <a name="monitoringsettings-resource-type"></a>monitoringSettings 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置在部署中控制自动监视和响应。

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

