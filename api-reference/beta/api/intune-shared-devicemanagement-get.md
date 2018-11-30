---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
ms.openlocfilehash: adc45ed789e3e636282fee851997c3fbcc8d8318
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044762"
---
# <a name="get-devicemanagement"></a>获取 deviceManagement

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。

## <a name="prerequisites"></a>先决条件

需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


| 权限&nbsp;类型&nbsp;(通过&nbsp;工作流) | 权限（从最高特权到最低特权） |
|:---|:---|
| 委派（工作或学校帐户） | |
| &nbsp;&nbsp; **Android 的工时** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **审核** | DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All |
| &nbsp;&nbsp; **公司术语** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **设备配置** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **电子 SIM** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **注册** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **防御** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **通知** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **入职培训** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **RBAC** | DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All |
| &nbsp;&nbsp; **远程访问** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **远程协助** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **电信支出管理** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **故障排除** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **Windows 信息保护** | DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持。|
| 应用程序 | 不支持。 |



## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a>响应

下面是响应的示例。 

注意： 为了简单起见，如下所示的响应对象可能被截断。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

返回属性适用于工作流。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```



