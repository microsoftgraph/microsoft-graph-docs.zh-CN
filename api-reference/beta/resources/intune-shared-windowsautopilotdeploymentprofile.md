---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows Autopilot Deployment配置文件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d3061cd127e83aed1ae5cf43ddf715decd9f40f5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444521"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a>windowsAutopilotDeploymentProfile 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows Autopilot Deployment配置文件

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsAutopilotDeploymentProfile](../api/intune-shared-windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|读取 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) 对象的属性和关系。|
|[分配操作](../api/intune-shared-windowsautopilotdeploymentprofile-assign.md)|无|尚未记录|
|**策略集**|
|[hasPayloadLinks 操作](../api/intune-shared-windowsautopilotdeploymentprofile-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|配置文件密钥|
|displayName|String|配置文件的名称|
|description|String|配置文件的说明|
|language|String|在设备上配置的语言|
|createdDateTime|DateTimeOffset|配置文件创建时间|
|lastModifiedDateTime|DateTimeOffset|上次修改时间的配置文件|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|开箱即用体验设置|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|注册状态屏幕设置|
|extractHardwareHash|Boolean|配置文件的 HardwareHash 提取|
|deviceNameTemplate|String|用于命名 AutoPilot 设备的模板。 这可以是自定义文本，也可以包含设备的序列号或随机生成的数字。 模板生成的文本总长度不得超过 15 个字符。|
|deviceType|[windowsAutopilotDeviceType](../resources/intune-enrollment-windowsautopilotdevicetype.md)|此配置文件适用的 AutoPilot 设备类型。 可取值为：`windowsPc`、`surfaceHub2`。|
|enableWhiteGlove|Boolean|为配置文件启用 Autopilot White Glove。|
|roleScopeTagIds|String collection|配置文件的作用域标记。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|**注册**|
|assignedDevices|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 集合|配置文件的已分配设备列表。|
|assignments|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) 集合|配置文件的组分配列表。|

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
  "deviceType": "String",
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```



