---
title: 创建 authoredNote
description: 创建新的 authoredNote 对象。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 116a09b703cc5f5ab30b2911eacfd1f1fe9593a3
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696349"
---
# <a name="create-authorednote"></a>创建 authoredNote
命名空间：microsoft.graph

创建新的 [authoredNote](../resources/authorednote.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|SubjectRightsRequest.ReadWrite.All*|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持|

>[!IMPORTANT]
>标有星号* (*) 当前不可用。 有关详细信息，请参阅[已知问题](/graph/known-issues#compliance)。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [authoredNote](../resources/authorednote.md) 对象的 JSON 表示形式。

下表显示创建 [authoredNote](../resources/authorednote.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|内容|[microsoft.graph.itemBody](../resources/itembody.md)|请求的注释内容|


## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [authoredNote](../resources/authorednote.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_authorednote_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
Content-Type: application/json
Content-length: 203

{
"content": 
  {
    "content": "String",
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

---



### <a name="response"></a>响应
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
    "id": "String (identifier)",
    "createdDateTime": "String (timestamp)",
    "author": { "@odata.type": "microsoft.graph.identitySet"},
    "content": {
          "@odata.type": "microsoft.graph.itemBody"
    }

}
```

