---
title: 创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId
description: 创建新的 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf3fc86212cc0c00f7152fee82ccc67912f2fe46
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259275"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyappversiondeviceid"></a>创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersionDeviceId
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId 对象的 JSON 表示形式。

下表显示创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析应用性能对象的唯一标识符。|
|deviceId|String|设备的 ID。|
|deviceDisplayName|String|设备的名称。|
|processedDateTime|DateTimeOffset|上次计算统计信息的日期和时间。|
|appName|String|应用程序名。|
|appDisplayName|String|应用程序的友好名称。|
|appPublisher|String|应用程序的发布者。|
|appVersion|String|应用程序的版本。|
|appCrashCount|Int32|应用的崩溃数。 有效值 -2147483648 2147483647|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersionDeviceId
Content-type: application/json
Content-length: 439

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "processedDateTime": "2017-01-01T00:03:22.2339319-08:00",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appVersion": "App Version value",
  "appCrashCount": 13
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 488

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId",
  "id": "2dad85e9-85e9-2dad-e985-ad2de985ad2d",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "processedDateTime": "2017-01-01T00:03:22.2339319-08:00",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appVersion": "App Version value",
  "appCrashCount": 13
}
```




