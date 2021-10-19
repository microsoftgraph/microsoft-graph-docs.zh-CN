---
title: 更新 importedAppleDeviceIdentityResult
description: 更新 importedAppleDeviceIdentityResult 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab44bef68cefcb51665c9fbdd53806fb7f257794
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60487483"
---
# <a name="update-importedappledeviceidentityresult"></a>更新 importedAppleDeviceIdentityResult

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [importedAppleDeviceIdentityResult 对象](../resources/intune-enrollment-importedappledeviceidentityresult.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象的 JSON 表示形式。

下表显示创建 [importedAppleDeviceIdentityResult 时所需的属性](../resources/intune-enrollment-importedappledeviceidentityresult.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|String|设备序列号 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|requestedEnrollmentProfileId|String|注册配置文件 ID 管理员打算在下一次注册期间应用到设备 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|向设备分配注册配置文件的时间 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|isSupervised|Boolean|指示 Apple 设备是否受监督。 详细信息位于： https://support.apple.com/en-us/HT202837 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple 设备发现源。 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。 可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。|
|isDeleted|Boolean|指示设备是否从 Apple Business Manager 中删除 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|createdDateTime|DateTimeOffset|设备的创建日期时间 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|设备的上次联系日期时间 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|说明|String|设备描述 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Intune 中的设备状态 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|平台|[平台](../resources/intune-enrollment-platform.md)|设备平台。 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|status|Boolean|导入的设备标识的状态|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 652

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```



