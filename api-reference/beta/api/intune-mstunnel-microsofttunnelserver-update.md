---
title: 更新 microsoftTunnelServer
description: 更新 microsoftTunnelServer 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 115faf5de18b113120540d96e954df2d7a0f04b2
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60486556"
---
# <a name="update-microsofttunnelserver"></a>更新 microsoftTunnelServer

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [microsoftTunnelServer 对象](../resources/intune-mstunnel-microsofttunnelserver.md) 的属性。

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
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象的 JSON 表示形式。

下表显示创建 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|MicrosoftTunnelServer 的 ID|
|displayName|String|MicrosoftTunnelServer 的显示名称|
|tunnelServerHealthStatus|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|MicrosoftTunnelServer 的运行状况状态。 可取值为：`unknown`、`healthy`、`unhealthy`、`warning`、`offline`、`upgradeInProgress` 或 `upgradeFailed`。|
|lastCheckinDateTime|DateTimeOffset|MicrosoftTunnelServer 上次签入时间|
|agentImageDigest|String|在此服务器上运行的当前代理映像的摘要 |
|serverImageDigest|String|在此服务器上运行的当前服务器映像的摘要 |



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
Content-type: application/json
Content-length: 312

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00",
  "agentImageDigest": "Agent Image Digest value",
  "serverImageDigest": "Server Image Digest value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 361

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "id": "b5cf0aee-0aee-b5cf-ee0a-cfb5ee0acfb5",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00",
  "agentImageDigest": "Agent Image Digest value",
  "serverImageDigest": "Server Image Digest value"
}
```



