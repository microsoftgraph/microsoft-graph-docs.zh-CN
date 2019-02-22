---
title: windowsAutopilotSettings 资源类型
description: windowsAutopilotSettings 资源表示用于将数据与 windows 设备数据同步服务同步的 Windows Autopilot 帐户。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b34d6edbed5bc98989ea70186b081d5c88a1c1b6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140514"
---
# <a name="windowsautopilotsettings-resource-type"></a>windowsAutopilotSettings 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

windowsAutopilotSettings 资源表示用于将数据与 windows 设备数据同步服务同步的 Windows Autopilot 帐户。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|读取[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性和关系。|
|[更新 windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。|
|[同步操作](../api/intune-enrollment-windowsautopilotsettings-sync.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|对象的 GUID|
|lastSyncDateTime|DateTimeOffset|包含 DDS 服务的上次数据同步日期时间。|
|lastManualSyncTriggerDateTime|DateTimeOffset|包含 DDS 服务的上次数据同步日期时间。|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|指示与设备数据同步 (DDS) 服务同步的状态。 可取值为：`unknown`、`inProgress`、`completed`、`failed`。|

## <a name="relationships"></a>Relationships
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




