---
title: 更新 userExperienceAnalyticsDeviceStartupHistory
description: 更新 userExperienceAnalyticsDeviceStartupHistory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4bf2ddc2ad60d850ba1511c6a1a7339a48326ec2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159666"
---
# <a name="update-userexperienceanalyticsdevicestartuphistory"></a>更新 userExperienceAnalyticsDeviceStartupHistory

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsDeviceStartupHistory 对象](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsDeviceStartupHistory 时所需的属性](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析设备启动历史记录的唯一标识符。|
|deviceId|String|用户体验分析设备 ID。|
|startTime|DateTimeOffset|用户体验分析设备启动开始时间。|
|coreBootTimeInMs|Int32|用户体验分析设备核心启动时间（以毫秒为单位）。|
|groupPolicyBootTimeInMs|Int32|用户体验分析设备组策略启动时间（以毫秒为单位）。|
|featureUpdateBootTimeInMs|Int32|用户体验分析设备功能更新时间（以毫秒为单位）。|
|totalBootTimeInMs|Int32|用户体验分析设备总启动时间（以毫秒为单位）。|
|groupPolicyLoginTimeInMs|Int32|用户体验分析设备组策略登录时间（以毫秒为单位）。|
|coreLoginTimeInMs|Int32|用户体验分析设备核心登录时间（以毫秒为单位）。|
|responsiveDesktopTimeInMs|Int32|用户体验分析响应式桌面时间（以毫秒为单位）。|
|totalLoginTimeInMs|Int32|用户体验分析设备总登录时间（以毫秒为单位）。|
|isFirstLogin|布尔|用户体验分析设备第一次登录。|
|isFeatureUpdate|布尔|用户体验分析设备启动记录是功能更新。|
|operatingSystemVersion|String|用户体验分析设备启动记录的操作系统版本。|
|restartCategory|[userExperienceAnalyticsOperatingSystemRestartCategory](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|操作系统重启类别。 可取值为：`unknown`、`restartWithUpdate`、`restartWithoutUpdate`、`blueScreen`、`shutdownWithUpdate`、`shutdownWithoutUpdate`、`longPowerButtonPress`、`bootError`、`update`。|
|restartStopCode|String|操作系统重新启动停止代码。 这将显示可用于查找蓝屏原因的 Bug 检查代码。|
|restartFaultBucket|String|操作系统重新启动故障存储桶。 故障存储桶用于查找有关系统崩溃的其他信息。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回响应代码和更新的用户 `200 OK` [ExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
Content-type: application/json
Content-length: 680

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 729

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "13357123-7123-1335-2371-351323713513",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```




