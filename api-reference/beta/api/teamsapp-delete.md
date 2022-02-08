---
title: 删除 teamsApp
description: '从Teams应用程序目录组织的应用程序目录中删除 (应用程序) 。 '
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: db01e3cab8f6e10b7f43ed6aefae0efb9975a9d4
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/08/2022
ms.locfileid: "62443196"
---
# <a name="delete-teamsapp"></a>删除 teamsApp

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD001 -->

从 [租户应用程序](../resources/teamsapp.md) 目录组织的应用程序目录中 (应用程序) 。 若要删除应用， **应用的 distributionMethod** 属性必须设置为 `organization`。

您还可以使用此 API 从评价过程中删除已提交的应用。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

>**注意：** 只有全局管理员可以调用此 API。 

| 权限类型                        | 权限（从最低特权到最高特权）|
|:----------------------------------     |:-------------|
| 委派（工作或学校帐户） | AppCatalog.Submit、AppCatalog.ReadWrite.All、Directory.ReadWrite.All** |
| 委派（个人 Microsoft 帐户） | 不支持。|
| 应用程序                            | 不支持。 |

> **注意**：标记为 ** 的权限仅支持向后兼容。 建议您将解决方案更新为使用不同的权限，并避免今后使用这些权限。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

若要从应用程序目录中删除应用程序，请运行以下操作：

```http
DELETE /appCatalogs/teamsApps/{id}
```

若要删除已提交但尚未批准的应用，请运行：

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a>请求标头

| 标头        | 值           |
|:--------------|:--------------  |
| Authorization | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

>**注意：** 使用从列表已发布 [的应用](./appcatalogs-list-teamsapps.md) 调用返回的 ID 来引用你要删除的应用。 请勿使用 zip 应用包清单中的 ID。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-teamsapp-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-teamsapp-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
