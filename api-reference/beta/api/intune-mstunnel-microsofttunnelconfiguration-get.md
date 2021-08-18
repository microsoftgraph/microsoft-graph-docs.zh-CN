---
title: 获取 microsoftTunnelConfiguration
description: 读取 microsoftTunnelConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c822a950bc98a336f935bd517c7f150fc3689f7193de6cf47a2701ded72dc538
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54171047"
---
# <a name="get-microsofttunnelconfiguration"></a>获取 microsoftTunnelConfiguration

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

读取 [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 对象的属性和关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、MicrosoftTunnelGateway.Read.All、MicrosoftTunnelGateway.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|MicrosoftTunnelGateway.Read.All、MicrosoftTunnelGateway.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
GET /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelConfiguration
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 876

{
  "value": {
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
    ]
  }
}
```




