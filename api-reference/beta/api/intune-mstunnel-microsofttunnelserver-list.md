---
title: 列出 microsoftTunnelServers
description: 列出 microsoftTunnelServer 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6a35fa3181d483e2db3d6052e983b159813e7bc
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347100"
---
# <a name="list-microsofttunnelservers"></a>列出 microsoftTunnelServers

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

列出 [microsoftTunnelServer 对象的属性和](../resources/intune-mstunnel-microsofttunnelserver.md) 关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftTunnelServer",
      "id": "b5cf0aee-0aee-b5cf-ee0a-cfb5ee0acfb5",
      "displayName": "Display Name value",
      "tunnelServerHealthStatus": "healthy",
      "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00",
      "agentImageDigest": "Agent Image Digest value",
      "serverImageDigest": "Server Image Digest value"
    }
  ]
}
```




