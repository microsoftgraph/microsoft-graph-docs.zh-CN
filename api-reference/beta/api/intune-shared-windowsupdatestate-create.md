---
title: 创建 windowsUpdateState
description: 创建新的 windowsUpdateState 对象。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ead882c17c4e37f3535b0a022a1d5914461749e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58794123"
---
# <a name="create-windowsupdatestate"></a>创建 windowsUpdateState

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）||
| &nbsp; &nbsp; **设备配置** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp; &nbsp; **软件更新** | DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序||
| &nbsp; &nbsp; **设备配置** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp; &nbsp; **软件更新** | DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 windowsUpdateState 对象的 JSON 表示形式。

下表显示创建 windowsUpdateState 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|这是实体的 ID。|
|deviceId|String|设备的 ID。|
|userId|String|用户的 ID。|
|deviceDisplayName|String|设备显示名称。|
|userPrincipalName|String|用户主体名称。|
|状态|[windowsUpdateStatus](../resources/intune-shared-windowsupdatestatus.md)|Windows udpate 状态。 可取值为：`upToDate`、`pendingInstallation`、`pendingReboot`、`failed`。|
|qualityUpdateVersion|字符串|质量更新设备的版本。|
|featureUpdateVersion|字符串|设备的当前功能更新版本。|
|lastScanDateTime|DateTimeOffset|更新代理执行Windows扫描的日期时间。|
|lastSyncDateTime|DateTimeOffset|设备上次与设备同步的日期Microsoft Intune。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "3d92af00-af00-3d92-00af-923d00af923d",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```






