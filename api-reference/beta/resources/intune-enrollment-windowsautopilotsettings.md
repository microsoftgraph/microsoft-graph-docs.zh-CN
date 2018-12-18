---
title: windowsAutopilotSettings 资源类型
description: WindowsAutopilotSettings 资源表示为与 Windows 设备数据同步服务的同步数据的 Windows 自动执行某些操作帐户。
author: tfitzmac
ms.openlocfilehash: d502af67cc1a68c56e1bdd74965e77224947b5d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344630"
---
# <a name="windowsautopilotsettings-resource-type"></a>windowsAutopilotSettings 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

WindowsAutopilotSettings 资源表示为与 Windows 设备数据同步服务的同步数据的 Windows 自动执行某些操作帐户。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|读取属性和[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的关系。|
|[更新 windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。|
|[同步操作](../api/intune-enrollment-windowsautopilotsettings-sync.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|对象的 GUID|
|lastSyncDateTime|DateTimeOffset|最后一个数据同步与 DD 服务的日期时间。|
|lastManualSyncTriggerDateTime|DateTimeOffset|最后一个数据同步与 DD 服务的日期时间。|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|指示与设备数据同步 (DD) 服务的同步状态。 可取值为：`unknown`、`inProgress`、`completed`、`failed`。|

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





