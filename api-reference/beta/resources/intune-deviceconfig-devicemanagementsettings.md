---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1009096aa25a504ba02b3c0cc2b8dc9eed6cf2dc
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291153"
---
# <a name="devicemanagementsettings-resource-type"></a>deviceManagementSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|允许设备无需签入即可保持符合性的天数。|
|isScheduledActionEnabled|Boolean|是否为规则的计划操作启用此功能。|
|secureByDefault|Boolean|它为 true 时，如果不存在目标符合性策略，则设备应为不符合。|
|enhancedJailBreak|Boolean|是否启用功能以用于增强的越狱检测。|
|deviceInactivityBeforeRetirementInDay|Int32|当设备在指定的天数内未签入时，可能会删除公司数据，并且设备不会管理。 有效值为 30 至 270|
|derivedCredentialProvider|[derivedCredentialProviderType](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|要用于此帐户的派生凭据提供程序。 可取值为：`notConfigured`、`entrustDataCard`、`purebred`、`xTec`、`intercede`。|
|derivedCredentialUrl|String|派生的凭据提供程序自助服务 URI。|
|androidDeviceAdministratorEnrollmentEnabled|Boolean|属性，用于确定是否为此帐户启用了 Android 设备管理员注册。|
|ignoreDevicesForUnsupportedSettingsEnabled|Boolean|属性，用于确定是否忽略某些型号的设备上不受支持的合规性设置。|
|enableLogCollection|Boolean|确定是否应该可以使用日志收集功能。|
|enableAutopilotDiagnostics|Boolean|确定是否启用 autopilot 诊断功能。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024,
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String",
  "androidDeviceAdministratorEnrollmentEnabled": true,
  "ignoreDevicesForUnsupportedSettingsEnabled": true,
  "enableLogCollection": true,
  "enableAutopilotDiagnostics": true
}
```




