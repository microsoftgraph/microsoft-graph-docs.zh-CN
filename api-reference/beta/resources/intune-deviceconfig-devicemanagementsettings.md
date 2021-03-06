---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cdf84f8adff40825ad0cd0792d8868b0ff76ed0b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283446"
---
# <a name="devicemanagementsettings-resource-type"></a>deviceManagementSettings 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|允许设备无需签入即可保持符合性的天数。|
|isScheduledActionEnabled|Boolean|是否为规则的计划操作启用此功能。|
|secureByDefault|Boolean|它为 true 时，如果不存在目标符合性策略，则设备应为不符合。|
|enhancedJailBreak|Boolean|功能是否已启用或不适用于增强的 jailbreak 检测。|
|deviceInactivityBeforeRetirementInDay|Int32|如果设备在指定天数内未签入，则可能会删除公司数据，并且设备将不受管理。 有效值为30至270|
|derivedCredentialProvider|[derivedCredentialProviderType](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|要用于此帐户的派生的凭据提供程序。 可取值为：`notConfigured`、`entrustDataCard`、`purebred`、`xTec`、`intercede`。|
|derivedCredentialUrl|字符串|派生的凭据提供程序自助服务 URI。|
|androidDeviceAdministratorEnrollmentEnabled|Boolean|用于确定是否为此帐户启用了 Android 设备管理员注册的属性。|
|ignoreDevicesForUnsupportedSettingsEnabled|Boolean|用于确定是否忽略某些型号的设备上不受支持的合规性设置的属性。|
|enableLogCollection|Boolean|确定是否应可使用 "日志收集" 功能。|

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
  "enableLogCollection": true
}
```




