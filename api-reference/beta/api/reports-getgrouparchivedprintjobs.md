---
title: reports： getGroupArchivedPrintJobs
description: 获取特定组的已存档打印作业的列表。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 875be990d0f97ebbe6e2c487926685829ee1d4eb
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944772"
---
# <a name="reports-getgrouparchivedprintjobs"></a>reports： getGroupArchivedPrintJobs

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取特定组的已存档打印作业的列表。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| Reports.Read.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getGroupArchivedPrintJobs(groupId=groupId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getGroupArchivedPrintJobs(groupId=groupId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a>请求标头
| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |

## <a name="function-parameters"></a>函数参数

| 参数     | 类型                 | 是否必需？ | 说明                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `groupId`     | `Edm.String`         | 是       | 要返回其数据的组的 ID。                              |
| `startDateTime` | `Edm.DateTimeOffset` | 否        | 开始日期 (包含) 数据的时间（含这两者）。 |
| `endDateTime`   | `Edm.DateTimeOffset` | 否        | 结束日期 (包含) 的数据时间段的结束日期（含这两者）。   |

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [archivedPrintJob](../resources/archivedprintjob.md) 对象集合。

## <a name="example"></a>示例
以下示例演示如何调用此 API。
##### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reports-getgrouparchivedprintjobs",
  "sampleKeys": ["016b5565-3bbf-4067-b9ff-4d68167eb1a6"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/getGroupArchivedPrintJobs(groupId='016b5565-3bbf-4067-b9ff-4d68167eb1a6',startDateTime=2021-05-24,endDateTime=2021-05-25)
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reports-getgrouparchivedprintjobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reports-getgrouparchivedprintjobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reports-getgrouparchivedprintjobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reports-getgrouparchivedprintjobs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.archivedPrintJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
  "description": "printJob: getGroupArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

