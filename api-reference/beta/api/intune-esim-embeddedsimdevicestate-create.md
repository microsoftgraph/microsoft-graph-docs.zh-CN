---
title: 创建 embeddedSIMDeviceState
description: 创建新的 embeddedSIMDeviceState 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 451f40d7ad23787311e4a0b9ed3c046cbe34b830
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413414"
---
# <a name="create-embeddedsimdevicestate"></a>创建 embeddedSIMDeviceState

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 embeddedSIMDeviceState 对象的 JSON 表示形式。

下表显示时创建 embeddedSIMDeviceState 所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|嵌入 SIM 设备状态的唯一标识符。 系统生成时创建分配值。|
|createdDateTime|DateTimeOffset|创建嵌入的 SIM 设备状态的时间。 生成的服务方。|
|modifiedDateTime|DateTimeOffset|上次修改嵌入的 SIM 设备状态的时间。 更新服务端。|
|lastSyncDateTime|DateTimeOffset|嵌入的 SIM 设备上次签入的时间。 更新服务端。|
|universalIntegratedCircuitCardIdentifier|String|通用集成电路卡标识符 (UICCID) 标识到配置文件是要部署的硬件。|
|deviceName|String|订阅已的设备名称设置如桌面 JOE|
|userName|String|订阅已设置到例如 joe@contoso.com 用户名|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|应用于该设备配置文件操作的状态。 可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。|
|stateDetails|String|字符串设置状态的说明。|



## <a name="response"></a>响应
如果成功，此方法返回`201 Created`响应代码和响应正文中的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "908884a3-84a3-9088-a384-8890a3848890",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```




