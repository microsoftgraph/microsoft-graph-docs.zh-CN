---
title: 报告： getUserArchivedPrintJobs
description: 获取特定用户的已存档打印作业的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 017488e472143d66b48ca33732c0ea1d6aa07475
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845440"
---
# <a name="reports-getuserarchivedprintjobs"></a>报告： getUserArchivedPrintJobs

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取特定用户的已存档打印作业的列表。

## <a name="permissions"></a>Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| 已阅读的用户。所有 |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getUserArchivedPrintJobs
GET /reports/getUserArchivedPrintJobs
```
## <a name="request-headers"></a>请求标头
| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}. Required. |

## <a name="function-parameters"></a>函数参数

| 参数     | 类型                 | 是否必需？ | Description                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `userId`      | `Edm.String`         | 是       | 要为其返回数据的用户的 ID。                               |
| `periodStart` | `Edm.DateTimeOffset` | 否        | 要在其中包含数据的时间段的开始日期（含）。 |
| `periodEnd`   | `Edm.DateTimeOffset` | 否        | 要在其中包含数据的时间段的结束日期（含）。   |

## <a name="response"></a>响应
如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[archivedPrintJob](../resources/archivedprintjob.md)对象集合。

## <a name="example"></a>示例
以下示例演示如何调用此 API。
##### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "reports-getuserarchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getUserArchivedPrintJobs(userId={id},periodStart=<timestamp>,periodEnd=<timestamp>)
```

##### <a name="response"></a>响应
下面展示了示例响应。
>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.archivedPrintJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 236

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printer": {
        "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6"
      },
      "createdBy": {},
      "processingState": "completed"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: getUserArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->