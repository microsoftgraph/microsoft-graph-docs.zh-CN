---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f2829a759266b4b0254077df78740a3f5394beb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59132587"
---
# <a name="update-devicemanagement"></a>更新 deviceManagement

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本的 API 可能会更改。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。

## <a name="prerequisites"></a>先决条件

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

请注意，权限因工作流而异。

| 工作流 &nbsp; &nbsp; (的权限 &nbsp; 类型)  | 权限（从最高特权到最低特权） |
|:---|:---|
| 委派（工作或学校帐户） ||
| &nbsp;&nbsp; **Android for Work** | DeviceManagementConfiguration.ReadWrite.All  |
| &nbsp; &nbsp; **审核** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **公司条款** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **设备配置** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp;**设备意图** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp;**电子 SIM 卡** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp;**注册** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Fencing** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **通知** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Odj** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **载入** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;**策略集** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **基于角色的访问控制 (RBAC)** | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp;**远程访问** | DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp;**远程协助** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **软件更新** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;**电信费用管理** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;**问题** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; **Windows 信息保护** | DeviceManagementApps.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。|
| 应用程序 ||
| &nbsp;&nbsp; **Android for Work** | DeviceManagementConfiguration.ReadWrite.All  |
| &nbsp; &nbsp; **审核** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **公司条款** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **设备配置** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp;**设备意图** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp;**电子 SIM 卡** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp;**注册** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Fencing** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **通知** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Odj** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **载入** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;**策略集** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **基于角色的访问控制 (RBAC)** | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp;**远程访问** | DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp;**远程协助** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **软件更新** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;**电信费用管理** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;**问题** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; **Windows 信息保护** | DeviceManagementApps.ReadWrite.All |

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
|接受|application/json|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的 JSON 表示形式。

下表显示创建 [deviceManagement](../resources/intune-shared-devicemanagement.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|设备的唯一标识符。|
|**设备配置**|
|intuneAccountId|GUID|给定租户的 Intune 帐户 ID|
|legacyPcManangementEnabled|Boolean|用于为此帐户启用非 MDM 托管旧版电脑管理的 属性。 此属性是只读的。|
|maximumDepTokens|Int32|允许每个租户使用的最大 DEP 令牌数。|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|帐户级别设置。|
|**设备管理**|
|accountMoveCompletionDateTime|DateTimeOffset|租户&之间移动时的日期。|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|管理员同意信息。|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|设备保护概述。|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|设备清理规则|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|租户移动设备管理订阅状态。 可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。|
|订阅|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|租户的订阅。 可取值为：`none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Windows 设备的恶意软件概述。|
|**载入**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。|

请求正文属性支持因工作流而异。

## <a name="response"></a>响应
如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是设备管理工作流之后的请求示例：

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

下面是一个响应示例。 

注意：为简洁起见，可能会截断此处显示的响应对象。 返回的属性因工作流和上下文而异。

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









