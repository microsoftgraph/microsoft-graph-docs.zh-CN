---
title: safeguardSettings 资源类型
description: 管理服务应用于部署中的设备的安全措施。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: af40a9aaa8001bda15f442dd7f79baac014168a2
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695529"
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

