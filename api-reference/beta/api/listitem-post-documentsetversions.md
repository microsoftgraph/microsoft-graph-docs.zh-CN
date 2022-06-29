---
title: 创建 documentSetVersion
description: 在列表中创建文档集项的新版本。
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 9965f40ef61031fd690d730fff2f9477081f81c9
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444158"
---
# <a name="create-documentsetversion"></a>创建 documentSetVersion
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[列表](../resources/list.md)中创建文[档集](../resources/documentsetversion.md)项的新版本。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All、Sites.Selected|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/documentSetVersions
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [documentSetVersion](../resources/documentsetversion.md) 对象的 JSON 表示形式。

创建 **documentSetVersion** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|注释|String|对捕获的版本进行注释。 可选。|
|shouldCaptureMinorVersion|Boolean|如果 `true`还捕获了次要版本的项目，则仅捕获主要版本。 可选。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [documentSetVersion](../resources/documentsetversion.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_documentsetversion"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/root/lists/Documents/items/2/documentSetVersions
Content-Type: application/json
Content-length: 70

{
  "comment": "v1",
  "shouldCaptureMinorVersion": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-documentsetversion-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-documentsetversion-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-documentsetversion-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-documentsetversion-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-documentsetversion-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-documentsetversion-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "name": "create_documentsetversion",
  "truncated": true,
  "@odata.type": "microsoft.graph.documentSetVersion"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "1",
    "lastModifiedDateTime": "2022-04-05T04:53:42Z",
    "comment": "v1",
    "createdDateTime": "2022-04-05T04:53:42Z",
    "shouldCaptureMinorVersion": false,
    "lastModifiedBy": {
        "user": {
            "displayName": "Tenant Admin User",
            "email": "admin@contoso.sharepoint.com"
        }
    },
    "items": [
        {
            "itemId": "a5d83ae7-8c3e-4a2c-bc3e-8f276db857bf",
            "versionId": "1.0"
        }
    ],
    "createdBy": {
        "user": {
            "displayName": "Tenant Admin User",
            "email": "admin@contoso.sharepoint.com"
        }
    }
}
```

