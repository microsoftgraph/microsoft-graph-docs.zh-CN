---
title: 更新 userExperienceAnalyticsBatteryHealthAppImpact
description: 更新 userExperienceAnalyticsBatteryHealthAppImpact 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6ecb7dc37f81804c04851c54eb9e7d3d07add883
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339932"
---
# <a name="update-userexperienceanalyticsbatteryhealthappimpact"></a>更新 userExperienceAnalyticsBatteryHealthAppImpact

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsBatteryHealthAppImpact 对象](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBatteryHealthAppImpact/{userExperienceAnalyticsBatteryHealthAppImpactId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsBatteryHealthAppImpact 时所需的属性](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池应用影响对象的唯一标识符。|
|activeDevices|Int32|14 天期间使用该应用的活动设备数。 有效值 -2147483648 2147483647|
|appName|String|应用名称。 例如：oltk.exe|
|appDisplayName|String|适用于显示名称用户友好应用程序。 例如：Outlook|
|appPublisher|String|应用发布者。 例如：Microsoft Corporation|
|isForegroundApp|Boolean|如果用户与应用有活动交互，则其为 true。|
|batteryUsagePercentage|双精度|当设备未接通交流电源时，此应用程序在 14 天内在租户中所有设备上计算出的总电池电源百分比。 百分比单位。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthAppImpact/{userExperienceAnalyticsBatteryHealthAppImpactId}
Content-type: application/json
Content-length: 308

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthAppImpact",
  "activeDevices": 13,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "isForegroundApp": true,
  "batteryUsagePercentage": 7.333333333333333
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 357

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthAppImpact",
  "id": "d2a9c89a-c89a-d2a9-9ac8-a9d29ac8a9d2",
  "activeDevices": 13,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "isForegroundApp": true,
  "batteryUsagePercentage": 7.333333333333333
}
```




