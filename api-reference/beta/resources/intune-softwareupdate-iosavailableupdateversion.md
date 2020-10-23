---
title: iosAvailableUpdateVersion 资源类型
description: iOS 可用的更新版本详细信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f2b94a098c70b6d4ac4105b31274f406f058c675
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696046"
---
# <a name="iosavailableupdateversion-resource-type"></a>iosAvailableUpdateVersion 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

iOS 可用的更新版本详细信息

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|productVersion|String|更新的版本。|
|postingDateTime|DateTimeOffset|更新的过帐日期。|
|expirationDateTime|DateTimeOffset|更新的到期日期。|
|supportedDevices|String collection|更新支持的设备的列表。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAvailableUpdateVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAvailableUpdateVersion",
  "productVersion": "String",
  "postingDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "supportedDevices": [
    "String"
  ]
}
```





