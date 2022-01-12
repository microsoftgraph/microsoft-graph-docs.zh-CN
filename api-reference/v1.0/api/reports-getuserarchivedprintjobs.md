---
title: reports： getUserArchivedPrintJobs
description: 获取特定用户的已存档打印作业的列表。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 50f48985beebb5230ece74fd62d6f793da364d6c
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863577"
---
# <a name="reportroot-getuserarchivedprintjobs"></a>reportRoot： getUserArchivedPrintJobs
命名空间：microsoft.graph

获取特定用户的已存档打印作业的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| Reports.Read.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getUserArchivedPrintJobs
```

## <a name="function-parameters"></a>函数参数

在请求 URL 中，提供以下带值的函数参数：

| 参数     | 类型                 | 是否必需？ | 说明                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `userId`      | `Edm.String`         | 是       | 要返回其数据的用户的 ID。                               |
| `startDateTime` | `Edm.DateTimeOffset` | 否        | 开始日期包括 (数据) 时间段的包含时间（含这两者）。|
| `endDateTime`   | `Edm.DateTimeOffset` | 不支持        | 结束日期包括 (数据) 时间段（含这两者）。|

>**注意：** 如果不需要值，则使用 null 值传递参数。
## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [archivedPrintJob](../resources/archivedprintjob.md) 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "reportroot_getuserarchivedprintjobs"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/getUserArchivedPrintJobs(userId='{id}',startDateTime=<timestamp>,endDateTime=<timestamp>)
```

### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.archivedPrintJob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "fe6ff85a-f0d3-4c4f-aec6-b9d5154356a1",
      "createdBy": {},
      "processingState": "completed"
    }
  ]
}
```

