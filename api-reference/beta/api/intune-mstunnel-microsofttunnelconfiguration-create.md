---
title: 创建 microsoftTunnelConfiguration
description: 创建新的 microsoftTunnelConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6da18e706ed377e6730eb414c575da9f7bd12206
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696124"
---
# <a name="create-microsofttunnelconfiguration"></a>创建 microsoftTunnelConfiguration

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 对象。

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
POST /deviceManagement/microsoftTunnelConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 microsoftTunnelConfiguration 对象的 JSON 表示形式。

下表显示创建 microsoftTunnelConfiguration 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|MicrosoftTunnelConfiguration 的 ID|
|displayName|String|MicrosoftTunnelConfiguration 的显示名称|
|说明|String|MicrosoftTunnelConfiguration 的说明|
|network|String|将用于为客户端分配虚拟地址的子网|
|dnsServers|String 集合|客户端将使用的 DNS 服务器|
|defaultDomainSuffix|字符串|客户端将使用的默认域附录|
|routesInclude|String 集合|服务器将路由的路由|
|routesExclude|String collection|服务器不会路由的路由子集|
|splitDNS|String 集合|使用提供的 dns 服务器解析的域|
|listenPort|Int32|TCP 和 UPD 将在服务器上侦听的端口|
|advancedSettings|[keyValuePair](../resources/intune-mstunnel-keyvaluepair.md) 集合|可应用于服务器的其他设置|
|lastUpdateDateTime|DateTimeOffset|上次更新 MicrosoftTunnelConfiguration 的时间|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。|
|disableUDPConnections|布尔值|设置 DisableUDPConnections 时，客户端和 VPN 服务器不会使用 DTLS 连接来命名数据。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations
Content-type: application/json
Content-length: 782

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "disableUDPConnections": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 831

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "id": "b8bdb469-b469-b8bd-69b4-bdb869b4bdb8",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "disableUDPConnections": true
}
```



