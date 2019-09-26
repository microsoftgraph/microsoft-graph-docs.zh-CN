---
title: 更新 userExperienceAnalyticsOverview
description: 更新 userExperienceAnalyticsOverview 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e90382c1a4e50aa7f880d836c592662c94ce587
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180081"
---
# <a name="update-userexperienceanalyticsoverview"></a>更新 userExperienceAnalyticsOverview

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性。

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
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的 JSON 表示形式。

下表显示创建[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|User experience analytics 概述的唯一标识符。|
|overallScore|Int32|用户体验分析总分。|
|deviceBootPerformanceOverallScore|Int32|User experience analytics 设备启动性能总分。|
|bestPracticesOverallScore|Int32|用户体验分析最佳实践总分。|
|insights|[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合|User experience analytics insights。|
|state|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|"用户体验分析" 类别的当前运行状况状态。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|



## <a name="response"></a>响应
如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 650

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 699

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData"
}
```




