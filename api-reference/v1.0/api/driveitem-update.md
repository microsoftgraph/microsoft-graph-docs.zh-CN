---
author: JeremyKelley
ms.date: 09/10/2017
title: 更新文件或文件夹
ms.localizationpriority: high
ms.prod: sharepoint
description: 按 ID 或路径更新 DriveItem 元数据。
doc_type: apiPageType
ms.openlocfilehash: 4af377c0f03436fa6364c347dce985f84fae3711
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59037983"
---
# <a name="update-driveitem-properties"></a>更新 DriveItem 属性

命名空间：microsoft.graph

按 ID 或路径更新 [DriveItem](../resources/driveitem.md) 元数据。

还可以通过更新项的 **parentReference** 属性，使用更新将 [项移动到](driveitem-move.md)其他父级。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All    |
|应用程序 | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a>可选的请求标头

| 名称          | 类型   | 说明                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | String | 如果包含此请求标头，且提供的 eTag（或 cTag）与文件夹上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的属性的值。

请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，应用不应包括尚未更改的属性。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [DriveItem](../resources/driveitem.md) 资源。

## <a name="example"></a>示例

本示例将 DriveItem 资源重命名为“new-file-name.docx”。


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "update-item", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

如果成功，此方法将在响应正文中返回 [driveItem][item-resource] 资源。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "name": "new-file-name.docx",
  "file": { }
}
```

## <a name="error-responses"></a>错误响应

请参阅[错误响应][error-response]，详细了解错误返回方式。

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": [
  ]
} -->

