---
title: 创建 windowsAutopilotDeviceIdentity
description: 创建新的 windowsAutopilotDeviceIdentity 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f1c533593c0730846f570b67ee1a31446bba16e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204035"
---
# <a name="create-windowsautopilotdeviceidentity"></a>创建 windowsAutopilotDeviceIdentity

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 windowsAutopilotDeviceIdentity 对象提供 JSON 表示形式。

下表显示了创建 windowsAutopilotDeviceIdentity 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Windows autopilot 设备的配置文件分配状态。 可取值为：`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending` 或 `failed`。|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|配置文件分配Windows autopilot 设备的详细状态。 可取值为：`none`、`hardwareRequirementsNotMet`、`surfaceHubProfileNotSupported`、`holoLensProfileNotSupported`、`windowsPcProfileNotSupported`、`surfaceHub2SProfileNotSupported` 或 `unknownFutureValue`。|
|deploymentProfileAssignedDateTime|DateTimeOffset|Windows autopilot 设备的配置文件设置时间。|
|groupTag|String|Windows autopilot 设备的组标记。|
|purchaseOrderIdentifier|String|Windows autopilot 设备的采购订单标识符。|
|serialNumber|String|Windows autopilot 设备序列号。|
|productKey|String|Windows autopilot 设备产品密钥。|
|manufacturer|String|Windows autopilot 设备的 Oem 制造商。|
|model|String|Windows autopilot 设备的模型名称。|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Intune autopilot 设备的Windows注册状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|lastContactedDateTime|DateTimeOffset|Intune Windows autopilot 设备的上次联系日期时间。|
|addressableUserName|String|可寻址用户名。|
|userPrincipalName|字符串|用户主体名称。|
|resourceName|String|资源名称。|
|skuNumber|String|SKU 编号|
|systemFamily|String|系统系列|
|azureActiveDirectoryDeviceId|字符串|AAD设备 ID - 要弃用|
|azureAdDeviceId|字符串|AAD设备 ID|
|managedDeviceId|字符串|托管设备 ID|
|displayName|String|显示名称|
|deviceAccountUpn|String|Surface Hub设备帐户更新|
|deviceAccountPassword|String|Surface Hub设备帐户密码|
|deviceFriendlyName|String|Surface Hub设备友好名称|
|remediationState|[windowsAutopilotDeviceRemediationState](../resources/intune-enrollment-windowsautopilotdeviceremediationstate.md)|设备修正状态。 可取值为：`unknown`、`noRemediationRequired`、`automaticRemediationRequired`、`manualRemediationRequired`、`unknownFutureValue`。|
|remediationStateLastModifiedDateTime|DateTimeOffset|Autopilot 设备的 RemediationState 设置时间。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 1371

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureAdDeviceId": "Azure Ad Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "deviceAccountUpn": "Device Account Upn value",
  "deviceAccountPassword": "Device Account Password value",
  "deviceFriendlyName": "Device Friendly Name value",
  "remediationState": "noRemediationRequired",
  "remediationStateLastModifiedDateTime": "2017-01-01T00:00:10.730021-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1420

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureAdDeviceId": "Azure Ad Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "deviceAccountUpn": "Device Account Upn value",
  "deviceAccountPassword": "Device Account Password value",
  "deviceFriendlyName": "Device Friendly Name value",
  "remediationState": "noRemediationRequired",
  "remediationStateLastModifiedDateTime": "2017-01-01T00:00:10.730021-08:00"
}
```




