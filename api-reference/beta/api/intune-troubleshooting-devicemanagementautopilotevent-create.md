---
title: 创建 deviceManagementAutopilotEvent
description: 创建新的 deviceManagementAutopilotEvent 对象。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d1197d1a542df099243a00d989c25273db124a07
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59116169"
---
# <a name="create-devicemanagementautopilotevent"></a>创建 deviceManagementAutopilotEvent

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 deviceManagementAutopilotEvent 对象的 JSON 表示形式。

下表显示创建 deviceManagementAutopilotEvent 时所需的属性。

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
|userPrincipalName|String|用于注册设备的用户主体名称。|
|windowsAutopilotDeploymentProfileDisplayName|String|Autopilot 配置文件名称。|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|注册状态，如已注册、已失败。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|windows10EnrollmentCompletionPageConfigurationDisplayName|String|注册状态页面配置文件名称|
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
|enrollmentFailureDetails|String|注册失败详细信息。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/v1/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1545

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "deviceId": "Device Id value",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
  "enrollmentType": "azureADJoinedWithAutopilotProfile",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "enrolled",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
  "deploymentState": "success",
  "deviceSetupStatus": "success",
  "accountSetupStatus": "success",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT3M21.5549443S",
  "deploymentTotalDuration": "PT1M43.5284261S",
  "devicePreparationDuration": "-PT1M32.1347897S",
  "deviceSetupDuration": "-PT2M57.2190107S",
  "accountSetupDuration": "-PT2M32.0507894S",
  "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
  "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1594

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
  "deviceId": "Device Id value",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
  "enrollmentType": "azureADJoinedWithAutopilotProfile",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "enrolled",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
  "deploymentState": "success",
  "deviceSetupStatus": "success",
  "accountSetupStatus": "success",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT3M21.5549443S",
  "deploymentTotalDuration": "PT1M43.5284261S",
  "devicePreparationDuration": "-PT1M32.1347897S",
  "deviceSetupDuration": "-PT2M57.2190107S",
  "accountSetupDuration": "-PT2M32.0507894S",
  "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
  "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```




