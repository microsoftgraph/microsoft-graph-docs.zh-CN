---
title: 笔记本：getRecentNotebooks
description: 获取登录用户访问的 recentNotebook 实例列表。
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: c37d09ba8a9b56379b10ff52391da6c0a98277a0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120398"
---
# <a name="notebook-getrecentnotebooks"></a>笔记本：getRecentNotebooks

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取登录用户访问的 [recentNotebook](../resources/recentnotebook.md) 实例列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All|
|委派（个人 Microsoft 帐户） | Notes.Create、Notes.Read、Notes.ReadWrite |
|应用程序 | Notes.Read.All、Notes.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

用户的 `{id | userPrincipalName}` 必须与用于发出请求的授权令牌中编码的用户一致。

## <a name="function-parameters"></a>函数参数

| 参数    | 类型   |Description|
|:---------------|:--------|:----------|
|includePersonalNotebooks|Boolean|添加用户拥有的笔记本。 若要添加用户拥有的笔记本，请设置为 `true`；否则，设置为 `false`。 如果不添加 `includePersonalNotebooks` 参数，请求会返回 `400` 错误响应。|

## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功响应，则返回 `200 OK`，其中包含 **recentNotebooks** 的 JSON 集合。

## <a name="example"></a>示例
以下示例演示如何调用此 API。

##### <a name="request"></a>请求
下面为请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/recent-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/recent-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/recent-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/recent-notebooks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/recent-notebooks-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/recent-notebooks-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
以下示例显示了相应的响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "name":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "name":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```


