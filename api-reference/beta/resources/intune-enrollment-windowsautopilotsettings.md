---
title: windowsAutopilotSettings 资源类型
description: windowsAutopilotSettings 资源表示一个Windows Autopilot 帐户，用于Windows设备数据同步服务的数据。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d79155c3642eee237fd4bda53ecb6650f5cfbe7e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039957"
---
# <a name="windowsautopilotsettings-resource-type"></a>windowsAutopilotSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

windowsAutopilotSettings 资源表示一个Windows Autopilot 帐户，用于Windows设备数据同步服务的数据。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|读取 [windowsAutopilotSettings 对象的属性和](../resources/intune-enrollment-windowsautopilotsettings.md) 关系。|
|[更新 windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|更新 [windowsAutopilotSettings 对象](../resources/intune-enrollment-windowsautopilotsettings.md) 的属性。|
|[同步操作](../api/intune-enrollment-windowsautopilotsettings-sync.md)|无|从适用于企业应用商店和其他门户启动所有 AutoPilot 注册设备的同步。 如果同步成功，此操作将返回"204 无内容"响应代码。 如果同步正在进行，则此操作将返回 409 冲突响应代码。  如果在上一个同步的 10 分钟内调用此同步操作，则此操作将返回 429"请求过多"响应代码。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|lastSyncDateTime|DateTimeOffset|DDS 服务的上次数据同步日期时间。|
|lastManualSyncTriggerDateTime|DateTimeOffset|DDS 服务的上次数据同步日期时间。|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|指示与 DDS 服务的设备数据 (同步) 状态。 可取值为：`unknown`、`inProgress`、`completed`、`failed`。|

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



