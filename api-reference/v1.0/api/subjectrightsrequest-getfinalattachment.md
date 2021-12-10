---
title: subjectRightsRequest： getFinalAttachment
description: 获取主题权限请求的最终附件。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 5b2ef398666d5a2883acf40a405da5371cb2adaa
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2021
ms.locfileid: "61403132"
---
# <a name="subjectrightsrequest-getfinalattachment"></a>subjectRightsRequest： getFinalAttachment
命名空间：microsoft.graph

获取主题权限请求的最终附件。 附件是一个 zip 文件，其中包含隐私管理员包含的所有文件。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|SubjectRightsRequest.Read.All、SubjectRightsRequest.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|不支持|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalAttachment
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数将重定向到包含 SAS Microsoft Azure blob 存储链接并返回 `302` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "subjectRightsRequest_getfinalattachment"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalAttachment
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/subjectrightsrequest-getfinalattachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/subjectrightsrequest-getfinalattachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/subjectrightsrequest-getfinalattachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/subjectrightsrequest-getfinalattachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 302 
```

