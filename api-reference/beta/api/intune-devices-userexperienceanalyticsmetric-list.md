---
title: 列出 userExperienceAnalyticsMetrics
description: 列出 userExperienceAnalyticsMetric 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ca4286a2a1c851348c0f4441150163231cd5bae
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256289"
---
# <a name="list-userexperienceanalyticsmetrics"></a>列出 userExperienceAnalyticsMetrics

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

列出 [userExperienceAnalyticsMetric 对象的属性和](../resources/intune-devices-userexperienceanalyticsmetric.md) 关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 226

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
      "id": "1371822e-822e-1371-2e82-71132e827113",
      "value": 1.6666666666666667,
      "unit": "Unit value"
    }
  ]
}
```




