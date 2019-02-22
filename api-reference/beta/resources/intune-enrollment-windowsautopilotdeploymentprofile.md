---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows Autopilot 部署配置文件
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3b815e0184ab9969af348338c07c3fabf0b0597
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168871"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a>windowsAutopilotDeploymentProfile 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows Autopilot 部署配置文件

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsAutopilotDeploymentProfile](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|读取[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)对象的属性和关系。|
|[assign 操作](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字串符号|配置文件键|
|displayName|字符串|配置文件的名称|
|说明|字符串|配置文件的说明|
|language|String|在设备上配置的语言|
|createdDateTime|DateTimeOffset|配置文件创建时间|
|lastModifiedDateTime|DateTimeOffset|配置文件上次修改时间|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|"开箱即用体验" 设置|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|注册状态屏幕设置|
|extractHardwareHash|布尔|配置文件的 HardwareHash 提取|
|deviceNameTemplate|字符串|用于命名 AutoPilot 设备的模板。 它可以是自定义文本, 也可以包含设备的序列号或随机生成的数字。 模板生成的文本的总长度不能超过15个字符。|
|enableWhiteGlove|布尔|为配置文件启用 Autopilot 白色 Glove。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignedDevices|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合|配置文件的已分配设备的列表。|
|assignments|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合|配置文件的组分配列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "String",
    "deviceUsageType": "String",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "String",
    "installProgressTimeoutInMinutes": 1024,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "String",
  "enableWhiteGlove": true
}
```




