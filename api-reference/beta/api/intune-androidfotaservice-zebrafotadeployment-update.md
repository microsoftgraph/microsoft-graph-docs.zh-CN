---
title: 更新 zebraFotaDeployment
description: 更新 zebraFotaDeployment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d4b1d42cb140fd1acbc485ffe4f7b8d5d98843d8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213154"
---
# <a name="update-zebrafotadeployment"></a>更新 zebraFotaDeployment

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) 对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
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
PATCH /deviceManagement/zebraFotaDeployments/{zebraFotaDeploymentId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) 对象提供 JSON 表示形式。

下表显示了创建 [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|在创建部署期间提供的系统生成的部署 ID。 仅当操作成功时才返回。|
|displayName|String|部署的人工可读名称。|
|说明|String|有关部署的人工可读说明。|
|deploymentSettings|[zebraFotaDeploymentSettings](../resources/intune-androidfotaservice-zebrafotadeploymentsettings.md)|表示创建部署所需的设置，例如部署类型、项目信息、下载和安装|
|deploymentAssignments|[androidFotaDeploymentAssignment](../resources/intune-androidfotaservice-androidfotadeploymentassignment.md) 集合|Android FOTA 分配的集合|
|deploymentStatus|[zebraFotaDeploymentStatus](../resources/intune-androidfotaservice-zebrafotadeploymentstatus.md)|表示 Zebra 的部署状态。 状态是部署的高级状态，而不是每个设备的详细状态。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/zebraFotaDeployments/{zebraFotaDeploymentId}
Content-type: application/json
Content-length: 1892

{
  "@odata.type": "#microsoft.graph.zebraFotaDeployment",
  "displayName": "Display Name value",
  "description": "Description value",
  "deploymentSettings": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings",
    "deviceModel": "Device Model value",
    "updateType": "latest",
    "timeZoneOffsetInMinutes": 7,
    "firmwareTargetBoardSupportPackageVersion": "Firmware Target Board Support Package Version value",
    "firmwareTargetPatch": "Firmware Target Patch value",
    "firmwareTargetOsVersion": "Firmware Target Os Version value",
    "scheduleMode": "scheduled",
    "scheduleDurationInDays": 6,
    "downloadRuleNetworkType": "wifi",
    "downloadRuleStartDateTime": "2016-12-31T23:59:33.2519835-08:00",
    "installRuleStartDateTime": "2017-01-01T00:02:31.1558076-08:00",
    "installRuleWindowStartTime": "11:57:19.2230000",
    "installRuleWindowEndTime": "11:58:38.5330000",
    "batteryRuleMinimumBatteryLevelPercentage": 8,
    "batteryRuleRequireCharger": true
  },
  "deploymentAssignments": [
    {
      "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment",
      "id": "Id value",
      "target": {
        "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
        "groupId": "Group Id value"
      }
    }
  ],
  "deploymentStatus": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus",
    "state": "createFailed",
    "totalDevices": 12,
    "totalCreated": 12,
    "totalScheduled": 14,
    "totalDownloading": 0,
    "totalAwaitingInstall": 4,
    "totalSucceededInstall": 5,
    "totalCanceled": 13,
    "totalUnknown": 12,
    "totalFailedDownload": 3,
    "totalFailedInstall": 2,
    "completeOrCanceledDateTime": "2016-12-31T23:59:29.651377-08:00",
    "cancelRequested": true,
    "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
  }
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1941

{
  "@odata.type": "#microsoft.graph.zebraFotaDeployment",
  "id": "8bbfa8a0-a8a0-8bbf-a0a8-bf8ba0a8bf8b",
  "displayName": "Display Name value",
  "description": "Description value",
  "deploymentSettings": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings",
    "deviceModel": "Device Model value",
    "updateType": "latest",
    "timeZoneOffsetInMinutes": 7,
    "firmwareTargetBoardSupportPackageVersion": "Firmware Target Board Support Package Version value",
    "firmwareTargetPatch": "Firmware Target Patch value",
    "firmwareTargetOsVersion": "Firmware Target Os Version value",
    "scheduleMode": "scheduled",
    "scheduleDurationInDays": 6,
    "downloadRuleNetworkType": "wifi",
    "downloadRuleStartDateTime": "2016-12-31T23:59:33.2519835-08:00",
    "installRuleStartDateTime": "2017-01-01T00:02:31.1558076-08:00",
    "installRuleWindowStartTime": "11:57:19.2230000",
    "installRuleWindowEndTime": "11:58:38.5330000",
    "batteryRuleMinimumBatteryLevelPercentage": 8,
    "batteryRuleRequireCharger": true
  },
  "deploymentAssignments": [
    {
      "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment",
      "id": "Id value",
      "target": {
        "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
        "groupId": "Group Id value"
      }
    }
  ],
  "deploymentStatus": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus",
    "state": "createFailed",
    "totalDevices": 12,
    "totalCreated": 12,
    "totalScheduled": 14,
    "totalDownloading": 0,
    "totalAwaitingInstall": 4,
    "totalSucceededInstall": 5,
    "totalCanceled": 13,
    "totalUnknown": 12,
    "totalFailedDownload": 3,
    "totalFailedInstall": 2,
    "completeOrCanceledDateTime": "2016-12-31T23:59:29.651377-08:00",
    "cancelRequested": true,
    "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
  }
}
```




