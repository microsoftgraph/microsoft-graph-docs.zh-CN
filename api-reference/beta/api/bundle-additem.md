---
author: JeremyKelley
ms.author: jeremyke
title: 将项目添加到捆绑包
description: 将项目添加到 Driveitem 捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c192014a00e3a2119691857c8350dc03d53e1980
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441051"
---
# <a name="add-item-to-a-bundle"></a>将项目添加到捆绑包

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将其他[driveItem][]从驱动器添加到[捆绑包][]中。

[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。                             |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All   |
|应用程序          | 不支持。                                           |

## <a name="http-request"></a>HTTP 请求

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明  |
|:------------- |:------------ |
| Authorization | 持有者 \{token\}。 必填。 |

## <a name="request-body"></a>请求正文

请求正文包括应添加到捆绑的子集合中的项的标识符。

## <a name="response"></a>响应

如果成功，响应为`204 No Content`。

请参阅[错误响应][error-response]主题，详细了解错误返回方式。

## <a name="example"></a>示例

### <a name="request"></a>请求

此请求将现有项添加到指定的捆绑包中。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add items to an existing bundle.",
  "keywords": "",
  "section": "documentation"
} -->
