---
title: win32LobAppRestartSettings 资源类型
description: 包含描述应用程序安装后重启协调的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: abf2935fea6023682f5aa045e1c241fefef7f05a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523483"
---
# <a name="win32lobapprestartsettings-resource-type"></a>win32LobAppRestartSettings 资源类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含描述应用程序安装后重启协调的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|gracePeriodInMinutes|Int32|在应用程序安装后重新启动设备之前要等待的分钟数。|
|countdownDisplayBeforeRestartInMinutes|Int32|为等待重新启动而显示倒计时对话框之前的重新启动时间的分钟数。|
|restartNotificationSnoozeDurationInMinutes|Int32|选择 "暂停" 按钮时暂停 "重新启动通知" 对话框的分钟数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRestartSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRestartSettings",
  "gracePeriodInMinutes": 1024,
  "countdownDisplayBeforeRestartInMinutes": 1024,
  "restartNotificationSnoozeDurationInMinutes": 1024
}
```



