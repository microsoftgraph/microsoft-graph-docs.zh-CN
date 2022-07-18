---
title: user： exportPersonalData
description: 提交由公司管理员发出的数据策略操作请求以导出组织用户的数据。
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e592061e5cd7b3838be4d036beb46d5df4594b62
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653502"
---
# <a name="user-exportpersonaldata"></a>user： exportPersonalData

命名空间：microsoft.graph

从公司管理员或应用程序提交数据策略操作请求以导出组织用户的数据。 此数据包括存储在OneDrive中的用户数据及其活动报告。 有关在遵守法规的同时导出数据的更多指导，请 [参阅数据主体请求、GDPR 和 CCPA](/compliance/regulatory/gdpr-data-subject-requests)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  User.Export.All  |
|委派（个人 Microsoft 帐户） |  不适用  |
|应用程序 | User.Export.All |

>**注意：** 仅当使用委派权限时，公司管理员才能执行导出。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a>请求标头
| 名称       | 说明 |
|:---------------|:----------|
| Authorization  | 持有者 {token}|

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明 |
|:---------------|:--------|:----------|
|storageLocation|String|这是一个共享访问签名 (SAS) Azure 存储帐户的 URL，应将数据导出到何处。|

## <a name="response"></a>响应
如果成功，此方法返回 `202 Accepted` 响应代码。 它不会在响应正文中返回任何内容。 响应包含以下标头。

| 名称       | 说明 |
|:---------------|:----------|
| Location  | 用于检查请求状态的 URL。 |
| Retry-After  | 时间段（以秒为单位）。 请求创建者应在提交请求以检查状态后等待这么长时间。 |


## <a name="example"></a>示例
##### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json

{
  "storageLocation": "storageLocation-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-exportpersonaldata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-exportpersonaldata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-exportpersonaldata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-exportpersonaldata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-exportpersonaldata-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-exportpersonaldata-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应

```http
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


