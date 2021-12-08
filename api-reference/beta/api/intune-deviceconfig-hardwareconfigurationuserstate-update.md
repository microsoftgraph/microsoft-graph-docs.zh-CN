---
title: 更新 hardwareConfigurationUserState
description: 更新 hardwareConfigurationUserState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 502e007407fc8df86f2db41d7f99b6685b6c4f27
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345367"
---
# <a name="update-hardwareconfigurationuserstate"></a>更新 hardwareConfigurationUserState

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [hardwareConfigurationUserState 对象](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md) 的属性。

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
PATCH /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/userRunStates/{hardwareConfigurationUserStateId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md) 对象的 JSON 表示形式。

下表显示创建 [hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|硬件配置脚本用户状态实体的键。 此属性是只读的。|
|upn|String|用户主体名称 (UPN)|
|userEmail|String|用户电子邮件地址|
|userName|String|用户名|
|lastStateUpdateDateTime|DateTimeOffset|上次执行硬件配置的时间戳|
|successfulDeviceCount|Int32|特定用户的成功设备计数|
|failedDeviceCount|Int32|特定用户的失败设备计数|
|pendingDeviceCount|Int32|特定用户的挂起设备计数。|
|errorDeviceCount|Int32|特定用户的错误设备计数。|
|notApplicableDeviceCount|Int32|不适用于特定用户的设备计数。|
|unknownDeviceCount|Int32|特定用户的未知设备计数。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/userRunStates/{hardwareConfigurationUserStateId}
Content-type: application/json
Content-length: 406

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationUserState",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 455

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationUserState",
  "id": "303ad215-d215-303a-15d2-3a3015d23a30",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2
}
```




