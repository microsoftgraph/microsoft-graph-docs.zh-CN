---
title: 更新 hardwareConfigurationDeviceState
description: 更新 hardwareConfigurationDeviceState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 06f56ede9e8c98471992dac96a5d7de0797bd18a
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630700"
---
# <a name="update-hardwareconfigurationdevicestate"></a>更新 hardwareConfigurationDeviceState

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [hardwareConfigurationDeviceState 对象](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) 的属性。

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
PATCH /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/deviceRunStates/{hardwareConfigurationDeviceStateId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) 对象的 JSON 表示形式。

下表显示创建 [hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|硬件配置脚本设备状态实体的键。 此属性是只读的。|
|deviceName|String|设备名称|
|osVersion|String|设备的操作系统版本 (例如 10.0.19042.1165、10.0.19042.1288 等) |
|upn|String|用户主体名称 (UPN)。|
|internalVersion|Int32|策略内部版本|
|lastStateUpdateDateTime|DateTimeOffset|执行硬件配置的最后时间戳|
|configurationState|[runState](../resources/intune-deviceconfig-runstate.md)|上次执行硬件配置后的配置状态。 可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。|
|configurationOutput|String|硬件配置执行的输出|
|configurationError|String|硬件配置执行中的错误|



## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/deviceRunStates/{hardwareConfigurationDeviceStateId}
Content-type: application/json
Content-length: 410

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationDeviceState",
  "deviceName": "Device Name value",
  "osVersion": "Os Version value",
  "upn": "Upn value",
  "internalVersion": 15,
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "configurationState": "success",
  "configurationOutput": "Configuration Output value",
  "configurationError": "Configuration Error value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 459

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationDeviceState",
  "id": "74b9fcd8-fcd8-74b9-d8fc-b974d8fcb974",
  "deviceName": "Device Name value",
  "osVersion": "Os Version value",
  "upn": "Upn value",
  "internalVersion": 15,
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "configurationState": "success",
  "configurationOutput": "Configuration Output value",
  "configurationError": "Configuration Error value"
}
```




