---
title: getHealthMetricTimeSeries 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 424d4213f252b262d2c82511eacfab78615c205c
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493681"
---
# <a name="gethealthmetrictimeseries-action"></a>getHealthMetricTimeSeries 操作

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/certificateConnectorDetails/{certificateConnectorDetailsId}/getHealthMetricTimeSeries
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|属性|类型|说明|
|:---|:---|:---|
|timeSeries|[timeSeriesParameter](../resources/intune-raimportcerts-timeseriesparameter.md)|尚未记录|



## <a name="response"></a>响应
如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [certificateConnectorHealthMetricValue](../resources/intune-raimportcerts-certificateconnectorhealthmetricvalue.md) 集合。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/certificateConnectorDetails/{certificateConnectorDetailsId}/getHealthMetricTimeSeries

Content-type: application/json
Content-length: 242

{
  "timeSeries": {
    "@odata.type": "microsoft.graph.timeSeriesParameter",
    "metricName": "Metric Name value",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "endDateTime": "2017-01-01T00:03:30.9241974-08:00"
  }
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 225

{
  "value": [
    {
      "@odata.type": "microsoft.graph.certificateConnectorHealthMetricValue",
      "dateTime": "2016-12-31T23:59:57.0735821-08:00",
      "successCount": 12,
      "failureCount": 12
    }
  ]
}
```



