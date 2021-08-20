---
title: 更新 embeddedSIMDeviceState
description: 更新嵌入SIMDeviceState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aea3a0bdb903dd350ec7d0d38e39aafc8934de23df3e004fb6f532275fe55a19
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54166412"
---
# <a name="update-embeddedsimdevicestate"></a>更新 embeddedSIMDeviceState

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新嵌入 [SIMDeviceState 对象](../resources/intune-esim-embeddedsimdevicestate.md) 的属性。

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
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [embeddedSIMDeviceState 对象的](../resources/intune-esim-embeddedsimdevicestate.md) JSON 表示形式。

下表显示创建 [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|嵌入式 SIM 卡设备状态的唯一标识符。 创建时分配的系统生成值。|
|createdDateTime|DateTimeOffset|嵌入式 SIM 卡设备状态的创建时间。 生成的服务器端。|
|modifiedDateTime|DateTimeOffset|上次修改嵌入式 SIM 卡设备状态的时间。 更新的服务器端。|
|lastSyncDateTime|DateTimeOffset|嵌入式 SIM 卡设备上次签入的时间。 更新的服务器端。|
|universalIntegratedCircuitCardIdentifier|String|通用集成电路卡标识符 (UI进行) 标识要部署配置文件的硬件。|
|deviceName|String|预配订阅的设备名称，例如 DESKTOP-JOE|
|userName|String|订阅预配到的用户名，例如 joe@contoso.com|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|应用于设备的配置文件操作的状态。 可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。|
|stateDetails|String|设置状态字符串说明。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` [的 embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
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
HTTP/1.1 200 OK
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




