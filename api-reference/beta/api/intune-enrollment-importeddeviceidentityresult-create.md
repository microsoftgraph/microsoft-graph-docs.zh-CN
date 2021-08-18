---
title: 创建 importedDeviceIdentityResult
description: 创建新的 importedDeviceIdentityResult 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: acdcc7cb26e65c0da8b05e646a4e43f60ffbc967a4239da2c47646acb990c466
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54173896"
---
# <a name="create-importeddeviceidentityresult"></a>创建 importedDeviceIdentityResult

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象。

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
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 importedDeviceIdentityResult 对象的 JSON 表示形式。

下表显示创建 importedDeviceIdentityResult 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|导入的设备标识的 ID 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentifier|String|导入的设备标识符 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|导入的设备标识的类型 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。 可取值为：`unknown`、`imei`、`serialNumber`。|
|lastModifiedDateTime|DateTimeOffset|说明的 Last Modified DateTime 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|createdDateTime|DateTimeOffset|设备的创建日期时间 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|设备的上次联系日期时间 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|description|字符串|设备描述 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Intune 中的设备状态 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|平台|[平台](../resources/intune-enrollment-platform.md)|设备平台。 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|status|布尔值|导入的设备标识的状态|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象。

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




