---
author: swapnil1993
title: 更新 contentType
description: 更新内容类型。
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 717520b09780d85d53e92f7b7a40ef68f7ac1610
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022524"
---
# <a name="update-contenttype"></a>更新 contentType
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
更新内容 [类型][contentType]。
  

## <a name="permissions"></a>Permissions

  

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

  

|权限类型 | 权限（从最低特权到最高特权） |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Manage.All、Sites.FullControl.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 |Sites.Manage.All、Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供要更新的 [contentType][] 资源的 JSON 表示形式。  

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [contentType][] 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contenttype"
}
-->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
Content-Type: application/json

{
   "name":"updatedCt",
   "documentSet":{
      "shouldPrefixNameToFile":true,
      "allowedContentTypes":[
         {
            "id":"0x0101",
            "name":"Document"
         }
      ],
      "defaultContents":[
         {
            "fileName":"a.txt",
            "contentType":{
               "id":"0x0101"
            }
         },
         {
            "fileName":"b.txt",
            "contentType":{
               "id":"0x0101"
            }
         }
      ],
      "sharedColumns":[
         {
            "name":"Description",
            "id":"cbb92da4-fd46-4c7d-af6c-3128c2a5576e"
         },
         {
            "name":"Address",
            "id":"fc2e188e-ba91-48c9-9dd3-16431afddd50"
         }
      ],
      "welcomePageColumns":[
         {
            "name":"Address",
            "id":"fc2e188e-ba91-48c9-9dd3-16431afddd50"
         }
      ]
   }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-contenttype-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "id":"0x0101009B237E76EF94DC49B4E58139041E7C60",
   "description":"",
   "eTag":"\"7\"",
   "group":"Custom Content Types",
   "hidden":false,
   "name":"testdoc",
   "parentId":"0x0101",
   "base":{
      "id":"0x0101",
      "name":"Document"
   }
}
```

[contentType]: ../resources/contentType.md
