---
title: 创建 userExperienceAnalyticsBatteryHealthOsPerformance
description: 创建新的 userExperienceAnalyticsBatteryHealthOsPerformance 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8042302c8e79ed0b117a4b6ddf201e7255915dbc
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697253"
---
# <a name="create-userexperienceanalyticsbatteryhealthosperformance"></a>创建 userExperienceAnalyticsBatteryHealthOsPerformance

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md) 对象。

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
POST /deviceManagement/userExperienceAnalyticsBatteryHealthOsPerformance
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 userExperienceAnalyticsBatteryHealthOsPerformance 对象的 JSON 表示形式。

下表显示创建 userExperienceAnalyticsBatteryHealthOsPerformance 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|用户体验分析电池运行状况操作系统性能对象的唯一标识符。|
|activeDevices|Int32|该操作系统版本的活动设备数。 有效值 -2147483648 to 2147483647|
|osVersion|String|操作系统的版本。|
|osBuildNumber|字符串|操作系统的生成号。|
|averageMaxCapacityPercentage|Int32|运行特定操作系统版本的所有设备的最大容量的平均值。 最大容量用于测量设备电池的完全充电容量与设计容量。 有效值 -2147483648 to 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|对于运行特定操作系统版本的所有设备，估计运行时的全费平均值。 单位（以分钟表示）。 有效值 -2147483648 to 2147483647|
|averageBatteryAgeInDays|Int32|在租户中运行特定操作系统版本的所有设备的电池使用时间平均值。 单位（以天表示）。 有效值 -2147483648 to 2147483647|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthOsPerformance
Content-type: application/json
Content-length: 310

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthOsPerformance",
  "activeDevices": 13,
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "averageMaxCapacityPercentage": 12,
  "averageEstimatedRuntimeInMinutes": 0,
  "averageBatteryAgeInDays": 7
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 359

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthOsPerformance",
  "id": "9fc871ad-71ad-9fc8-ad71-c89fad71c89f",
  "activeDevices": 13,
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "averageMaxCapacityPercentage": 12,
  "averageEstimatedRuntimeInMinutes": 0,
  "averageBatteryAgeInDays": 7
}
```



