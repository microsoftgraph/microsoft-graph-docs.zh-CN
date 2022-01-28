---
title: teamworkSystemConfiguration 资源类型
description: 表示有关已启用Microsoft Teams配置的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dd22015f77cb65d2be52da8877f9808b73e2cac1
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262332"
---
# <a name="teamworksystemconfiguration-resource-type"></a>teamworkSystemConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已启用Microsoft Teams配置[的详细信息](../resources/teamworkdevice.md)。 不适用于Microsoft Teams 会议室设备。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|dateTimeConfiguration|[teamworkDateTimeConfiguration](../resources/teamworkdatetimeconfiguration.md)|设备的日期和时间配置。|
|defaultPassword|String|设备的默认密码。 只写。|
|deviceLockTimeout|期限|设备锁定超时（以秒表示）。|
|isDeviceLockEnabled|Boolean|`True` 如果设备锁定已启用。|
|isLoggingEnabled|Boolean|`True` 如果启用日志记录。|
|isPowerSavingEnabled|Boolean|`True` 如果启用节电功能。|
|isScreenCaptureEnabled|Boolean|`True` 如果启用屏幕捕获。|
|isSilentModeEnabled|Boolean|`True` 如果启用静默模式。|
|language|String|设备的语言选项。|
|lockPin|String|解锁设备的引脚。 只写。|
|loggingLevel|String|设备的日志记录级别。|
|networkConfiguration|[teamworkNetworkConfiguration](../resources/teamworknetworkconfiguration.md)|设备的网络配置。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSystemConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSystemConfiguration",
  "dateTimeConfiguration": {
    "@odata.type": "microsoft.graph.teamworkDateTimeConfiguration"
  },
  "defaultPassword": "String",
  "deviceLockTimeout": "String (duration)",
  "isDeviceLockEnabled": "Boolean",
  "isLoggingEnabled": "Boolean",
  "isPowerSavingEnabled": "Boolean",
  "isScreenCaptureEnabled": "Boolean",
  "isSilentModeEnabled": "Boolean",
  "language": "String",
  "lockPin": "String",
  "loggingLevel": "String",
  "networkConfiguration": {
    "@odata.type": "microsoft.graph.teamworkNetworkConfiguration"
  }
}
```

