---
title: teamworkConfiguredPeripheral 资源类型
description: 表示有关为启用了 Microsoft Teams 配置的外围设备的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 07a25c847acb1b9b7e3584b2a1a5ef86d7bff046
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262435"
---
# <a name="teamworkconfiguredperipheral-resource-type"></a>teamworkConfiguredPeripheral 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关为启用了 Microsoft Teams 设备的外围设备[的详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isOptional|Boolean|`True` 如果当前外设是可选的。 如果设置为 `false`，则此属性还用作计算设备运行状况的一部分。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|外设|[teamworkPeripheral](../resources/teamworkperipheral.md)|有关连接的外围设备的详细信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConfiguredPeripheral"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConfiguredPeripheral",
  "isOptional": "Boolean"
}
```

