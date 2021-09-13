---
title: 创建 androidManagedAppRegistration
description: 创建新的 androidManagedAppRegistration 对象。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26cb767ae744866da8924c7e0206e1aae5e02dc9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59065146"
---
# <a name="create-androidmanagedappregistration"></a>创建 androidManagedAppRegistration

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 androidManagedAppRegistration 对象的 JSON 表示形式。

下表显示了创建 androidManagedAppRegistration 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|lastSyncDateTime|DateTimeOffset|上次应用与管理服务同步的日期和时间。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|applicationVersion|String|应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|managementSdkVersion|String|应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|platformVersion|String|操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceType|String|主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceTag|String|应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。 不保证在所有情况下与应用关联。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceName|String|主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|managedDeviceId|String|主机设备的托管设备标识符。 即使托管主机设备，值也可以为空。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|azureADDeviceId|String|主机Azure Active Directory的设备标识符。 即使已注册主机设备，值Azure Active Directory为空。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceModel|String|当前应用注册的设备型号 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceManufacturer|String|当前应用注册的设备制造商 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|flaggedReasons|[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) 集合|标记应用注册的零个或多个原因。 例如， 在根设备上运行的应用 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)。 可取值为：`none`、`rootedDevice`、`androidBootloaderUnlocked`、`androidFactoryRomModified`。|
|userId|String|此应用注册所属的用户 ID。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|id|String|实体的键。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|version|String|实体的版本。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|patchVersion|String|当前 android 应用注册的修补程序版本|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 879

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 987

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```



