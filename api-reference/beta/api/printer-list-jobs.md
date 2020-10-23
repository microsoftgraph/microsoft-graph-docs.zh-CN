---
title: 列出打印机的 printJobs
description: 检索与打印机关联的打印作业的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6f1f056c0cb3dbcd9ffbd10627c9d3a673cf116d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690782"
---
# <a name="list-printjobs-for-a-printer"></a>列出打印机的 printJobs

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索与 [打印机](../resources/printer.md)关联的打印作业的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

若要使用通用打印服务，用户或应用程序的租户必须具有活动的通用打印订阅、授予 " [获取打印机](printer-get.md) 访问" 权限的权限以及下表中列出的权限之一。 登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。

若要从其他用户读取打印作业，则已登录用户必须是打印管理员，并且必须是 PrintJob、PrintJob、PrintJob 或 ReadWriteBasic。所有权限的 User.readbasic.all。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| PrintJob、PrintJob、user.readbasic.all、PrintJob、PrintJob、ReadWriteBasic、all、PrintJob、PrintJob、ReadWriteBasic、PrintJob、、、、all |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| PrintJob、PrintJob、PrintJob、all、all、All 和 All。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

* 默认情况下，" **documents** " 属性将从响应中省略。 若要同时为每个打印作业返回 [printDocuments](../resources/printdocument.md) 的列表，请使用 `$expand=documents` 。
* 此方法支持通过创建打印作业的用户对其进行筛选。 使用 `$filter=createdBy/userPrincipalName eq '{upn}'` ，其中 **{upn}** 是关联用户的 [用户主体名称](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) 。

### <a name="exceptions"></a>Exceptions
某些运算符不受支持： `$count` 、 `$search` 、 `$filter` 。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printJob](../resources/printjob.md) 对象集合。
## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```

---

### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 461

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs",
  "value": [
    {
      "id": "5182",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "processingState": "completed",
        "processingStateDescription": "The print job has completed successfully and no further processing will take place."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
