---
title: safeguardSettings 资源类型
description: 管理服务应用于部署中的设备的安全措施。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d3c276a07483b42e513266077ef1ada3bc516d47
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792118"
---
# <a name="safeguardsettings-resource-type"></a>safeguardSettings 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

管理服务应用于部署中的设备的安全措施。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|disabledSafeguardProfiles|[microsoft.graph.windowsUpdates.safeguardProfile](../resources/windowsupdates-safeguardprofile.md) 集合|要按设备忽略的安全措施列表。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.safeguardSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.safeguardSettings",
  "disabledSafeguardProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.safeguardProfile"
    }
  ]
}
```

