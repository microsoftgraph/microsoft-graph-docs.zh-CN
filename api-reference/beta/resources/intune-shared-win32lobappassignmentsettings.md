---
title: win32LobAppAssignmentSettings 资源类型
description: 包含用于将 Win32 LOB 移动应用分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 21e5e592465be9b1663d79136989740fcfe245666f46448ed304c51b392a557a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54219701"
---
# <a name="win32lobappassignmentsettings-resource-type"></a>win32LobAppAssignmentSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于将 Win32 LOB 移动应用分配给组的属性。


继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|通知|[win32LobAppNotification](../resources/intune-shared-win32lobappnotification.md)|此应用分配的通知状态。 可取值为：`showAll`、`showReboot`、`hideAll`。|
|restartSettings|[win32LobAppRestartSettings](../resources/intune-shared-win32lobapprestartsettings.md)|要应用于此应用分配的重启设置。|
|installTimeSettings|[mobileAppInstallTimeSettings](../resources/intune-shared-mobileappinstalltimesettings.md)|要应用于此应用分配的安装时间设置。|
|deliveryOptimizationPriority|[win32LobAppDeliveryOptimizationPriority](../resources/intune-shared-win32lobappdeliveryoptimizationpriority.md)|此应用分配的传递优化优先级。 国家云环境不支持此设置。 可取值为：`notConfigured`、`foreground`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String",
  "restartSettings": {
    "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
    "gracePeriodInMinutes": 1024,
    "countdownDisplayBeforeRestartInMinutes": 1024,
    "restartNotificationSnoozeDurationInMinutes": 1024
  },
  "installTimeSettings": {
    "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
    "useLocalTime": true,
    "startDateTime": "String (timestamp)",
    "deadlineDateTime": "String (timestamp)"
  },
  "deliveryOptimizationPriority": "String"
}
```




