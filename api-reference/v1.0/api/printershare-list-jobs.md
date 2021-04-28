---
title: 列出 printerShare 的 printJobs
description: 检索与打印共享关联的打印作业列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7899640922cd5f8ba38d11bba03c485dbb6099bd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053914"
---
# <a name="list-printjobs-for-a-printershare"></a>列出 printerShare 的 printJobs
命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

检索与 [printerShare](../resources/printershare.md)关联的打印作业列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予 [获取 printerShare](printershare-get.md) 访问权限的权限以及下表中列出的权限之一。

若要从其他用户读取打印作业，登录的用户需要是打印管理员，并且具有 PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All 或 PrintJob.ReadWrite.All 权限。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| PrintJob.ReadBasic、PrintJob.Read、PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/jobs
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

* 默认情况下 **，响应** 中将省略 documents 属性。 若要同时返回每个 [打印作业的 printDocuments](../resources/printdocument.md) 列表，请使用 `$expand=documents` 。
* 此方法支持按创建打印作业的用户筛选打印作业。 使用 `$filter=createdBy/userPrincipalName eq '{upn}'` ，其中 **{upn}** 是关联 [用户](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) 的用户主体名称。

### <a name="exceptions"></a>Exceptions
不支持某些运算符 `$count` `$search` ：、。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printJob](../resources/printjob.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printjob_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printjob-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printjob-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printjob-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printjob-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printJob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares('f37141d9-0afb-484f-96d3-0ef0a679e6c1')/jobs",
  "value": [
    {
      "id": "103",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {        
      },
      "status": {
        "state": "completed",
        "description": "The print job has completed successfully and no further processing will take place.",
        "details": [          
        ],
        "isAcquiredByPrinter": true
      },
      "configuration": {        
      },
      "redirectedTo": null,
      "redirectedFrom": null,
      "isFetchable": false
    }
  ]
}
```

