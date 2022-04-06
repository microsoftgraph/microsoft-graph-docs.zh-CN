---
author: JeremyKelley
title: 删除捆绑包
description: 删除 driveItems 捆绑包
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b574c73db2f4e0dd71d0e2e5c6685b58f8ad8143
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561592"
---
# <a name="delete-bundle"></a>删除捆绑包

命名空间：microsoft.graph

使用 [driveItems][] 的 id 删除捆绑 **包**。请注意，使用此方法删除捆绑包会永久删除该捆绑包，并且不会将其移动到回收站。
但是，它不会删除捆绑包引用的项目。
它们将保留在父文件夹中。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。                             |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All   |
|应用程序          | 不支持。                                           |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明  |
|:------------- |:------------ |
| Authorization | 持有者 \{token\}。必需。 |
| if-match      | eTag。 可选。 如果包含此请求标头，并且提供的 eTag (或 cTag `412 Precondition Failed`) 与捆绑包上的当前标记不匹配，将返回响应，并且不会删除捆绑包。

## <a name="request-body"></a>请求正文

请勿为此方法提供请求正文。

## <a name="response"></a>响应

如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。

有关错误响应的信息，请参阅 [错误响应][error-response]。

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```

### <a name="response"></a>响应

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[bundle]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a bundle from OneDrive",
  "keywords": "delete,existing bundle,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Delete"
} -->


