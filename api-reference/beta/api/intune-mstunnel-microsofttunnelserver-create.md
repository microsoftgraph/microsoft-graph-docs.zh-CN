---
title: 创建 microsoftTunnelServer
description: 创建新的 microsoftTunnelServer 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 146de9c8b03d2934ad6507b5adf2aecc3d778d75
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301527"
---
# <a name="create-microsofttunnelserver"></a>创建 microsoftTunnelServer

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 microsoftTunnelServer 对象的 JSON 表示形式。

下表显示创建 microsoftTunnelServer 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|MicrosoftTunnelServer 的 Id|
|displayName|字符串|MicrosoftTunnelServer 的显示名称|
|tunnelServerHealthStatus|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|MicrosoftTunnelServer 的运行状况状态。 可取值为：`unknown`、`healthy`、`unhealthy`、`warning`、`offline`、`upgradeInProgress` 或 `upgradeFailed`。|
|lastCheckinDateTime|DateTimeOffset|上次签入的 MicrosoftTunnelServer|



## <a name="response"></a>响应
如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "id": "b5cf0aee-0aee-b5cf-ee0a-cfb5ee0acfb5",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```




