---
title: 创建 deviceInstallState
description: 创建新的 deviceInstallState 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dfc1adae0175dcdf2c19d90d54bf597316919994
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990899"
---
# <a name="create-deviceinstallstate"></a>创建 deviceInstallState

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 deviceInstallState 对象的 JSON 表示形式。

下表显示创建 deviceInstallState 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|deviceName|String|设备名称。|
|deviceId|String|设备 ID。|
|lastSyncDateTime|DateTimeOffset|上次同步日期和时间。|
|installState|[installState](../resources/intune-books-installstate.md)|电子图书的安装状态。 可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。|
|errorCode|String|安装失败的错误代码。|
|osVersion|String|操作系统版本。|
|osDescription|String|操作系统说明。|
|userName|String|设备用户名。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```





