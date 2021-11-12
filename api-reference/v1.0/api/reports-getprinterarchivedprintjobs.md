---
title: reports： getPrinterArchivedPrintJobs
description: 获取已排队等待特定打印机的存档打印作业的列表。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 2ca0f329fa3378c4ed51355371b214dbcfb6a9f8
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60940499"
---
# <a name="reportroot-getprinterarchivedprintjobs"></a>reportRoot： getPrinterArchivedPrintJobs
命名空间：microsoft.graph

获取已排队等待特定打印机的存档打印作业 [的列表](../resources/printer.md)。

## <a name="permissions"></a>Permissions
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
GET /reports/getPrinterArchivedPrintJobs
```

## <a name="function-parameters"></a>函数参数

| 参数     | 类型                 | 是否必需？ | 说明                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | 是       | 要返回其数据的打印机的 ID。                            |
| `startDateTime` | `Edm.DateTimeOffset` | 否        | 开始日期 (包含) 数据的时间（含这两者）。 |
| `endDateTime`   | `Edm.DateTimeOffset` | 否        | 结束日期包括 (数据) 时间段的结束日期（含这两者）。   |

## <a name="request-headers"></a>请求头
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
  "name": "reportroot_getprinterarchivedprintjobs"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/getPrinterArchivedPrintJobs(printerId='{id}',startDateTime=<timestamp>,endDateTime=<timestamp>)
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

