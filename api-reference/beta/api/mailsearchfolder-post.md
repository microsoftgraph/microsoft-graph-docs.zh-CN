---
title: 创建 mailSearchFolder
description: 使用此 API 在指定用户的邮箱中创建新的 mailSearchFolder。
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2b791d4636f78c000a95d00bfd2e3d864d566881
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60934099"
---
# <a name="create-mailsearchfolder"></a>创建 mailSearchFolder

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在指定的[用户的邮箱中创建新的 mailSearchFolder。](../resources/mailsearchfolder.md)

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
|委派（工作或学校帐户） | Mail.ReadWrite    |
|委派（个人 Microsoft 帐户） | Mail.ReadWrite    |
|应用程序 | Mail.ReadWrite |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

在查询 URL 中将父文件夹指定为文件夹 ID 或已知文件夹名称。 有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。

## <a name="request-headers"></a>请求头

| 标头 | 值 |
|:-------|:------|
| 授权 | `Bearer {token}`. 必需。 |
| Content-Type | `application/json`. 必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数 | 类型 | 说明 |
|:----------|:-----|:------------|
| @odata.type | String | 要创建的文件夹的类型。 设置为"microsoft.graph.mailSearchFolder"。 |
| displayName | String | 新文件夹的显示名称。|
| includeNestedFolders | Boolean | 指示如何在搜索中遍历邮箱文件夹层次结构。 `true` 意味着应该执行深层搜索，以在 **sourceFolderIds** 中显式指定的每个文件夹的层次结构中包括子文件夹。 `false` 表示仅对 **sourceFolderIds** 中显式指定的每个文件夹进行浅表搜索。 |
| sourceFolderIds | String 集合 | 应缩小的邮箱文件夹。 |
| filterQuery | String | 用于筛选邮件的 OData 查询。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [mailSearchFolder](../resources/mailsearchfolder.md) 对象。

## <a name="example"></a>示例

#### <a name="request"></a>请求

下面是请求的一个示例 - 它将创建主题中包含字符串"weekly digest"的邮件的搜索文件夹。 搜索文件夹位于应用指定筛选器查询的同一文件夹下。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADYAAAIBDAAAAA=="],
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Weekly digests",
  "includeNestedFolders": true,
  "sourceFolderIds": ["AQMkADYAAAIBDAAAAA=="],
  "filterQuery": "contains(subject, 'weekly digest')"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders('AQMkADYAAAIBDAAAAA%3D%3D')/childFolders/$entity",
    "@odata.type": "#microsoft.graph.mailSearchFolder",
    "id": "AAMkADYfRAAAZg1yTAAA=",
    "displayName": "Weekly digests",
    "parentFolderId": "AQMkADYAAAIBDAAAAA==",
    "childFolderCount": 0,
    "unreadItemCount": 0,
    "totalItemCount": 0,
    "wellKnownName": null,
    "isSupported": true,
    "includeNestedFolders": true,
    "sourceFolderIds": [
        "AQMkADYAAAIBDAAAAA=="
    ],
    "filterQuery": "contains(subject, 'weekly digest')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


