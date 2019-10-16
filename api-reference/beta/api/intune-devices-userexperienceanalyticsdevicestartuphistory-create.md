---
title: 创建 userExperienceAnalyticsDeviceStartupHistory
description: 创建新的 userExperienceAnalyticsDeviceStartupHistory 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d36442808380f408998b8dedaf5d89d45acb0982
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529198"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a>创建 userExperienceAnalyticsDeviceStartupHistory

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象。

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
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 userExperienceAnalyticsDeviceStartupHistory 对象的 JSON 表示形式。

下表显示创建 userExperienceAnalyticsDeviceStartupHistory 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|User experience analytics 设备启动历史记录的唯一标识符。|
|deviceId|String|User experience analytics 设备 id。|
|startTime|DateTimeOffset|用户体验分析设备启动开始时间。|
|coreBootTimeInMs|Int32|User experience analytics device core boot time （以毫秒为单位）。|
|groupPolicyBootTimeInMs|Int32|User experience analytics Device group policy boot time （以毫秒为单位）。|
|featureUpdateBootTimeInMs|Int32|User experience analytics 设备功能更新时间（以毫秒为单位）。|
|totalBootTimeInMs|Int32|User experience analytics 设备总启动时间（以毫秒为单位）。|
|groupPolicyLoginTimeInMs|Int32|User experience analytics 设备组策略登录时间（以毫秒为单位）。|
|coreLoginTimeInMs|Int32|User experience analytics device core login time （以毫秒为单位）。|
|totalLoginTimeInMs|Int32|User experience analytics 设备总登录时间（以毫秒为单位）。|
|isFirstLogin|Boolean|User experience analytics 设备第一次登录。|



## <a name="response"></a>响应
如果成功，此方法在响应`201 Created`正文中返回响应代码和[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 407

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
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 456

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
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true
}
```






