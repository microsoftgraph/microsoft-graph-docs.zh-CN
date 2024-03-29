---
title: 更新 userExperienceAnalyticsOverview
description: 更新 userExperienceAnalyticsOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f646d1e1cb2ed530ea3d9eb9152bd544bc87c4c5
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292044"
---
# <a name="update-userexperienceanalyticsoverview"></a>更新 userExperienceAnalyticsOverview

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsOverview 对象](../resources/intune-devices-userexperienceanalyticsoverview.md) 的属性。

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
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsOverview 时所需的属性](../resources/intune-devices-userexperienceanalyticsoverview.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析概述的唯一标识符。|
|overallScore|Int32|用户体验分析总体分数。|
|deviceBootPerformanceOverallScore|Int32|用户体验分析设备启动性能总体分数。|
|bestPracticesOverallScore|Int32|用户体验分析最佳实践总体分数。|
|workFromAnywhereOverallScore|Int32|用户体验分析从任意位置工作总体分数。|
|appHealthOverallScore|Int32|用户体验分析应用运行状况总体分数。|
|resourcePerformanceOverallScore|Int32|用户体验分析资源性能总体分数。|
|batteryHealthOverallScore|Int32|用户体验分析电池运行状况总体分数。|
|insights|[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合|用户体验分析见解。|
|state|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析概述的当前运行状况。 可能的值是：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|deviceBootPerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"BootPerformance"类别的当前运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|bestPracticesHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"BestPractices"类别的当前运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|workFromAnywhereHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"WorkFromAnywhere"类别的当前运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|appHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"BestPractices"类别的当前运行状况。 可能的值是：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|resourcePerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"ResourcePerformance"类别的当前运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|batteryHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"BatteryHealth"类别的当前运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|



## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 1085

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "workFromAnywhereOverallScore": 12,
  "appHealthOverallScore": 5,
  "resourcePerformanceOverallScore": 15,
  "batteryHealthOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData",
  "workFromAnywhereHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceHealthState": "insufficientData",
  "batteryHealthState": "insufficientData"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1134

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "workFromAnywhereOverallScore": 12,
  "appHealthOverallScore": 5,
  "resourcePerformanceOverallScore": 15,
  "batteryHealthOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData",
  "workFromAnywhereHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceHealthState": "insufficientData",
  "batteryHealthState": "insufficientData"
}
```




