---
title: 创建 authoredNote
description: 创建新的 authoredNote 对象。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: eca3fb56abb6d524bd54201d09b37474ae333c26
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461574"
---
# <a name="create-authorednote"></a>创建 authoredNote
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [authoredNote](../resources/authorednote.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|SubjectRightsRequest.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

[!INCLUDE [subject-rights-request-privacy-deprecate](../../includes/subject-rights-request-privacy-deprecate.md)]

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/subjectRightsRequests/{subjectRightsRequestId}/notes
POST /privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [authoredNote](../resources/authorednote.md) 对象的 JSON 表示形式。

下表显示了创建 [authoredNote](../resources/authorednote.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|内容|[microsoft.graph.itemBody](../resources/itembody.md)|请求的笔记内容。|


## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [authoredNote](../resources/authorednote.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_authorednote_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
Content-Type: application/json

{
    "content": {
        "content": "Please take a look at the files tagged with follow up",
        "contentType": "text"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-authorednote-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-authorednote-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-authorednote-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-authorednote-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-authorednote-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authoredNote"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "D450C4F9-CC18-4784-9406-9372F4E05F7B",
    "createdDateTime": "2022-05-10T22:42:28Z",
    "author": {
        "user": {
            "id": "1B761ED2-AA7E-4D82-9CF5-C09D737B6167",
            "displayName": "srradmin@contoso.com"
        }
    },
    "content": {
        "content": "Please take a look at the files tagged with follow up",
        "contentType": "text"
    }
}
```

