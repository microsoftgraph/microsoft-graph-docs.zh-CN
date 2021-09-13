---
title: win32LobAppAssignmentSettings 资源类型
description: 包含用于将 Win32 LOB 移动应用分配给组的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f94cd9ddcfe6c4136a1ee427cf2290a50792290
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072433"
---
# <a name="win32lobappassignmentsettings-resource-type"></a>win32LobAppAssignmentSettings 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于将 Win32 LOB 移动应用分配给组的属性。


继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|通知|[win32LobAppNotification](../resources/intune-apps-win32lobappnotification.md)|此应用分配的通知状态。 可取值为：`showAll`、`showReboot`、`hideAll`。|
|restartSettings|[win32LobAppRestartSettings](../resources/intune-apps-win32lobapprestartsettings.md)|要应用于此应用分配的重启设置。|
|installTimeSettings|[mobileAppInstallTimeSettings](../resources/intune-apps-mobileappinstalltimesettings.md)|要应用于此应用分配的安装时间设置。|
|deliveryOptimizationPriority|[win32LobAppDeliveryOptimizationPriority](../resources/intune-apps-win32lobappdeliveryoptimizationpriority.md)|此应用分配的传递优化优先级。 国家云环境不支持此设置。 可取值为：`notConfigured`、`foreground`。|

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




