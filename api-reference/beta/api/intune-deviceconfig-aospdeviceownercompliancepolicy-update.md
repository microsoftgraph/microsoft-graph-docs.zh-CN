---
title: 更新 aospDeviceOwnerCompliancePolicy
description: 更新 aospDeviceOwnerCompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 41a729fbdf959c4727255432f667311f7187573a
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262331"
---
# <a name="update-aospdeviceownercompliancepolicy"></a>更新 aospDeviceOwnerCompliancePolicy

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [aospDeviceOwnerCompliancePolicy 对象](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) 对象的 JSON 表示形式。

下表显示创建 [aospDeviceOwnerCompliancePolicy 时所需的属性](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md)。

|属性|类型|说明|
|:---|:---|:---|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|id|字符串|实体的键。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|version|Int32|设备配置的版本。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|osMinimumVersion|String|最低 Android 版本。|
|osMaximumVersion|String|最高 Android 版本。|
|minAndroidSecurityPatchLevel|String|最低 Android 安全修补程序级别。|
|securityBlockJailbrokenDevices|Boolean|设备不得越狱或取得 root 权限。|
|passwordRequired|Boolean|需要密码才可解锁设备。|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|密码中的字符类型。 可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。|
|passwordMinutesOfInactivityBeforeLock|Int32|在需要密码之前不活动的分钟数。 有效值为 1 到 8640|
|passwordMinimumLength|Int32|最短密码长度。 有效值为 4 至 16|
|storageRequireEncryption|Boolean|要求对 Android 设备加密。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 636

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "securityBlockJailbrokenDevices": true,
  "passwordRequired": true,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumLength": 5,
  "storageRequireEncryption": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 808

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "0837b942-b942-0837-42b9-370842b93708",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "securityBlockJailbrokenDevices": true,
  "passwordRequired": true,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumLength": 5,
  "storageRequireEncryption": true
}
```




