---
title: deviceManagementAutopilotEvent 资源类型
description: 表示 Autopilot 流事件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d438723ab14cb9fd47828bbaba3b45ccbf5f7f13
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266798"
---
# <a name="devicemanagementautopilotevent-resource-type"></a>deviceManagementAutopilotEvent 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 Autopilot 流事件。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementAutopilotEvents](../api/intune-troubleshooting-devicemanagementautopilotevent-list.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 集合|列出 [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 对象的属性和关系。|
|[获取 deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-get.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|读取 [deviceManagementAutopilotEvent 对象的属性和](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 关系。|
|[创建 deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-create.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|创建新的 [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 对象。|
|[删除 deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-delete.md)|无|删除 [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)。|
|[更新 deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-update.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|更新 [deviceManagementAutopilotEvent 对象](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID|
|deviceId|String|与对象关联的设备 ID|
|eventDateTime|DateTimeOffset|事件发生的时间。|
|deviceRegisteredDateTime|DateTimeOffset|设备注册日期。|
|enrollmentStartDateTime|DateTimeOffset|设备注册开始日期。|
|enrollmentType|[windowsAutopilotEnrollmentType](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|注册类型。 可取值为：`unknown`、`azureADJoinedWithAutopilotProfile`、`offlineDomainJoined`、`azureADJoinedUsingDeviceAuthWithAutopilotProfile`、`azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`、`azureADJoinedWithOfflineAutopilotProfile`、`azureADJoinedWithWhiteGlove`、`offlineDomainJoinedWithWhiteGlove`、`offlineDomainJoinedWithOfflineAutopilotProfile`。|
|deviceSerialNumber|String|设备序列号。|
|managedDeviceName|String|托管设备名称。|
|userPrincipalName|字符串|用于注册设备的用户主体名称。|
|windowsAutopilotDeploymentProfileDisplayName|String|Autopilot 配置文件名称。|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|注册状态，如已注册、已失败。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|windows10EnrollmentCompletionPageConfigurationDisplayName|字符串|注册状态页面配置文件名称|
|windows10EnrollmentCompletionPageConfigurationId|String|注册状态页面配置文件 ID|
|deploymentState|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|部署状态，如 Success、Failure、InProgress、SuccessWithTimeout。 可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`、`notAttempted` 或 `disabled`。|
|deviceSetupStatus|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|注册状态页设备设置阶段的部署状态。 可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`、`notAttempted` 或 `disabled`。|
|accountSetupStatus|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|注册状态页帐户设置阶段的部署状态。 可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`、`notAttempted` 或 `disabled`。|
|osVersion|String|设备操作系统版本。|
|deploymentDuration|期限|Autopilot 部署持续时间（包括注册）。|
|deploymentTotalDuration|期限|从注册到桌面屏幕的总部署持续时间。|
|devicePreparationDuration|期限|设备注册所花费的时间。|
|deviceSetupDuration|期限|在设备 ESP 上花费的时间。|
|accountSetupDuration|期限|在用户 ESP 中花费的时间。|
|deploymentStartDateTime|DateTimeOffset|部署开始时间。|
|deploymentEndDateTime|DateTimeOffset|部署结束时间。|
|targetedAppCount|Int32|目标应用程序计数。|
|targetedPolicyCount|Int32|目标策略计数。|
|enrollmentFailureDetails|字符串|注册失败详细信息。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|policyStatusDetails|[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 集合|此设备的策略和应用程序状态详细信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAutopilotEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "String (identifier)",
  "deviceId": "String",
  "eventDateTime": "String (timestamp)",
  "deviceRegisteredDateTime": "String (timestamp)",
  "enrollmentStartDateTime": "String (timestamp)",
  "enrollmentType": "String",
  "deviceSerialNumber": "String",
  "managedDeviceName": "String",
  "userPrincipalName": "String",
  "windowsAutopilotDeploymentProfileDisplayName": "String",
  "enrollmentState": "String",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "String",
  "windows10EnrollmentCompletionPageConfigurationId": "String",
  "deploymentState": "String",
  "deviceSetupStatus": "String",
  "accountSetupStatus": "String",
  "osVersion": "String",
  "deploymentDuration": "String (duration)",
  "deploymentTotalDuration": "String (duration)",
  "devicePreparationDuration": "String (duration)",
  "deviceSetupDuration": "String (duration)",
  "accountSetupDuration": "String (duration)",
  "deploymentStartDateTime": "String (timestamp)",
  "deploymentEndDateTime": "String (timestamp)",
  "targetedAppCount": 1024,
  "targetedPolicyCount": 1024,
  "enrollmentFailureDetails": "String"
}
```




