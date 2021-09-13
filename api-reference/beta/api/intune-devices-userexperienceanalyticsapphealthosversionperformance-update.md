---
title: 更新 userExperienceAnalyticsAppHealthOSVersionPerformance
description: 更新 userExperienceAnalyticsAppHealthOSVersionPerformance 对象的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 015c1863dfd50044460702adb512020b278ad9ec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59034566"
---
# <a name="update-userexperienceanalyticsapphealthosversionperformance"></a>更新 userExperienceAnalyticsAppHealthOSVersionPerformance

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsAppHealthOSVersionPerformance 对象](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
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
PATCH /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance/{userExperienceAnalyticsAppHealthOSVersionPerformanceId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsAppHealthOSVersionPerformance 时所需的属性](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析操作系统版本性能对象的唯一标识符。|
|osVersion|String|设备上安装的操作系统版本。|
|osBuildNumber|String|设备上安装的操作系统内部版本号。|
|activeDeviceCount|Int32|操作系统版本的活动设备的数量。 有效值 -2147483648 2147483647|
|meanTimeToFailureInMinutes|Int32|操作系统版本的失败平均时间（分钟）。 有效值 -2147483648 2147483647|
|osVersionAppHealthScore|双精度|操作系统版本的应用运行状况分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|osVersionAppHealthStatus|String|操作系统版本的总体应用运行状况状态。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance/{userExperienceAnalyticsAppHealthOSVersionPerformanceId}
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 406

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "id": "7c28e16b-e16b-7c28-6be1-287c6be1287c",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```



