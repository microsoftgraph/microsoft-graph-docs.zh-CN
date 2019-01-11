---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e88b6379e340865adeb41bb0430fd8eecc8f0b69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860681"
---
# <a name="update-devicemanagement"></a>更新 deviceManagement

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


| 权限&nbsp;类型&nbsp;(通过&nbsp;工作流) | 权限（从最高特权到最低特权） |
|:---|:---|
| 委派（工作或学校帐户） |
| &nbsp;&nbsp;审核 | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp;公司术语 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;公司注册 | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp;&nbsp;设备配置 | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp;设备管理 | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp;终结点保护 | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp;通知 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;入职培训 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;基于角色的访问控制 | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp;远程协助 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;电信支出管理 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;疑难解答 | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; Windows 信息保护 | DeviceManagementApps.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。|
| 应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的 JSON 表示形式。

下表显示创建 [deviceManagement](../resources/intune-shared-devicemanagement.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|设备唯一标识符|
|**设备配置**|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|帐户级别设置。|
|**设备管理**|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|租户移动设备管理订阅状态。 可能的值为： `pending`， `active`， `warning`， `disabled`， `deleted`， `blocked`， `lockedOut`。|
|**入职培训**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。|

请求正文属性支持根据工作流而有所不同。

## <a name="response"></a>响应
如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
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
```

### <a name="response"></a>响应

下面是一个响应示例。 注意：为简洁起见，可能会截断此处展示的响应对象。 返回的属性根据工作流和上下文而有所不同。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
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
```



