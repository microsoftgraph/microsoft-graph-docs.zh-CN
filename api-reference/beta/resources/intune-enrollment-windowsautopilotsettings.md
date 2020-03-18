---
title: windowsAutopilotSettings 资源类型
description: WindowsAutopilotSettings 资源表示用于将数据与 Windows 设备数据同步服务同步的 Windows Autopilot 帐户。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 073c6431ed0ef817fa0349805e93601e7b31f882
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783359"
---
# <a name="windowsautopilotsettings-resource-type"></a>windowsAutopilotSettings 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

WindowsAutopilotSettings 资源表示用于将数据与 Windows 设备数据同步服务同步的 Windows Autopilot 帐户。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|读取[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性和关系。|
|[更新 windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。|
|[同步操作](../api/intune-enrollment-windowsautopilotsettings-sync.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|lastSyncDateTime|DateTimeOffset|包含 DDS 服务的上次数据同步日期时间。|
|lastManualSyncTriggerDateTime|DateTimeOffset|包含 DDS 服务的上次数据同步日期时间。|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|指示与设备数据同步（DDS）服务同步的状态。 可取值为：`unknown`、`inProgress`、`completed`、`failed`。|

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



