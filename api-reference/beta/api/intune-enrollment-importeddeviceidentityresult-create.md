---
title: 创建 importedDeviceIdentityResult
description: 创建新的 importedDeviceIdentityResult 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05f3880d005d78463c3225b0eef501dba5e21299
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416270"
---
# <a name="create-importeddeviceidentityresult"></a>创建 importedDeviceIdentityResult

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 importedDeviceIdentityResult 对象的 JSON 表示形式。

下表显示时创建 importedDeviceIdentityResult 所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|来自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)导入的设备的标识继承的 id|
|importedDeviceIdentifier|String|导入设备标识符继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)导入设备标识继承的类型。 可取值为：`unknown`、`imei`、`serialNumber`。|
|lastModifiedDateTime|DateTimeOffset|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)的说明继承的上次修改日期时间|
|createdDateTime|DateTimeOffset|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)创建设备继承的日期时间|
|lastContactedDateTime|DateTimeOffset|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)设备继承的最后一个联系日期时间|
|说明|String|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)设备继承说明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)中 Intune 继承的设备的状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|platform|[平台](../resources/intune-enrollment-platform.md)|设备的平台。 继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|status|Boolean|导入的设备标识的状态|



## <a name="response"></a>响应
如果成功，此方法返回`201 Created`响应代码和响应正文中的[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```




