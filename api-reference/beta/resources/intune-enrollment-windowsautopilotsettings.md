---
title: windowsAutopilotSettings 资源类型
description: WindowsAutopilotSettings 资源表示用于将数据与 Windows 设备数据同步服务同步的 Windows Autopilot 帐户。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f6e65e2c898cbaaaf9d77b00cbf056d4cf369af
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288626"
---
# <a name="windowsautopilotsettings-resource-type"></a>windowsAutopilotSettings 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

WindowsAutopilotSettings 资源表示用于将数据与 Windows 设备数据同步服务同步的 Windows Autopilot 帐户。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[获取 windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|读取 [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) 对象的属性和关系。|
|[更新 windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|更新 [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) 对象的属性。|
|[同步操作](../api/intune-enrollment-windowsautopilotsettings-sync.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|对象的 GUID|
|lastSyncDateTime|DateTimeOffset|包含 DDS 服务的上次数据同步日期时间。|
|lastManualSyncTriggerDateTime|DateTimeOffset|包含 DDS 服务的上次数据同步日期时间。|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|指示与设备数据同步 (DDS) 服务同步的状态。 可取值为：`unknown`、`inProgress`、`completed`、`failed`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```




