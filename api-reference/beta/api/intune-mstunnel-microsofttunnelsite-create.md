---
title: 创建 microsoftTunnelSite
description: 创建新的 microsoftTunnelSite 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8db705b90d16bf46d03d94c0ba3d405b792ee87b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341962"
---
# <a name="create-microsofttunnelsite"></a>创建 microsoftTunnelSite

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象。

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
POST /deviceManagement/microsoftTunnelSites
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 microsoftTunnelSite 对象的 JSON 表示形式。

下表显示创建 microsoftTunnelSite 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|MicrosoftTunnelSite 的 ID|
|displayName|String|MicrosoftTunnelSite 的显示名称|
|说明|String|MicrosoftTunnelSite 的说明|
|publicAddress|String|MicrosoftTunnelSite 的公共域名或 IP 地址|
|upgradeWindowUtcOffsetInMinutes|Int32|网站时区表示为与 UTC 的分钟偏移量|
|upgradeWindowStartTime|TimeOfDay|网站的升级窗口一天中的开始时间|
|upgradeWindowEndTime|TimeOfDay|网站的升级窗口结束时间|
|upgradeAutomatically|布尔值|网站的自动升级设置。 True 表示自动升级，false 表示手动控制|
|upgradeAvailable|布尔值|如果升级可用，则其为 True|
|internalNetworkProbeUrl|String|MicrosoftTunnelSite 的内部网络访问探测器 URL|
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。|



## <a name="response"></a>响应
如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites
Content-type: application/json
Content-length: 524

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "upgradeWindowUtcOffsetInMinutes": 15,
  "upgradeWindowStartTime": "12:01:27.3030000",
  "upgradeWindowEndTime": "11:57:17.9830000",
  "upgradeAutomatically": true,
  "upgradeAvailable": true,
  "internalNetworkProbeUrl": "https://example.com/internalNetworkProbeUrl/",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 573

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "b2f7dc3e-dc3e-b2f7-3edc-f7b23edcf7b2",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "upgradeWindowUtcOffsetInMinutes": 15,
  "upgradeWindowStartTime": "12:01:27.3030000",
  "upgradeWindowEndTime": "11:57:17.9830000",
  "upgradeAutomatically": true,
  "upgradeAvailable": true,
  "internalNetworkProbeUrl": "https://example.com/internalNetworkProbeUrl/",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




