---
title: win32LobAppRestartSettings 资源类型
description: 包含描述应用安装后重启协调的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1db011486f1ec26afcc7e045afd2e1be1b553ec7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757828"
---
# <a name="win32lobapprestartsettings-resource-type"></a>win32LobAppRestartSettings 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含描述应用安装后重启协调的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|gracePeriodInMinutes|Int32|应用安装后重启设备之前等待的分钟数。|
|countdownDisplayBeforeRestartInMinutes|Int32|重启时间前显示挂起重启的倒计时器对话框的分钟数。|
|restartNotificationSnoozeDurationInMinutes|Int32|选择"暂停"按钮时暂停重新启动通知对话框的分钟数。|

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




