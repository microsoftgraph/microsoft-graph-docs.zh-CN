---
title: ediscoveryReviewTag： asHierarchy
description: 将标记列为层次结构*
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 0202282a840c7221a373f054d1ba6cfd23fd65e5
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094805"
---
# <a name="ediscoveryreviewtag-ashierarchy"></a>ediscoveryReviewTag： asHierarchy
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

显示标记层次结构的列表标记。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.Read.All、eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/tags/asHierarchy
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 `200 OK` 响应代码和 [microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewtagthis.ashierarchy"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags/asHierarchy
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoveryreviewtagthisashierarchy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoveryreviewtagthisashierarchy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoveryreviewtagthisashierarchy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/ediscoveryreviewtagthisashierarchy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryReviewTag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(ediscoveryReviewTag)",
    "@odata.count": 5,
    "value": [
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
            "displayName": "My tag API 2",
            "description": "Use Graph API to create tags (updated)",
            "lastModifiedDateTime": "2022-05-30T00:27:41.6407249Z",
            "childSelectability": "Many",
            "id": "062de822f17a4a2e9b833aa3f6c37108",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "childTags": []
        },
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
            "displayName": "Responsive",
            "description": "",
            "lastModifiedDateTime": "2022-05-23T19:41:24.4237284Z",
            "childSelectability": "One",
            "id": "d3d99dc704a74801b792b3e1e722aa0d",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "childTags": []
        },
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
            "displayName": "Not responsive",
            "lastModifiedDateTime": "2022-05-23T19:41:31.3381716Z",
            "childSelectability": "One",
            "id": "ced26633616a434abd83762d49a25a6c",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "childTags": []
        },
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
            "displayName": "Processing",
            "description": "Determine whether to outsource processing",
            "lastModifiedDateTime": "2022-05-23T19:46:03.8746996Z",
            "childSelectability": "Many",
            "id": "d8580989505c4fb3a25b845013697cf7",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "childTags": []
        },
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
            "displayName": "My tag API",
            "description": "Use Graph API to create tags",
            "lastModifiedDateTime": "2022-05-23T19:58:26.1573076Z",
            "childSelectability": "Many",
            "id": "7c6cc351-fb90-431f-8562-1b607a3144a4",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                },
                "application": {
                    "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                    "displayName": "Graph Explorer"
                }
            },
            "childTags": []
        }
    ]
}
```

