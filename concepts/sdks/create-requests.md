---
title: 使用 Microsoft SDK Graph API 调用
description: 提供有关使用 SDK Graph Microsoft HTTP 请求的说明。
ms.localizationpriority: medium
author: DarrelMiller
ms.openlocfilehash: d2d7b1f1a19c1a0a890bab6ab6a8c51ba7ec47a0
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226357"
---
<!-- markdownlint-disable MD025 -->

# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a>使用 Microsoft SDK Graph API 调用

Microsoft Graph SDK 服务库提供了一个客户端类，可以用作创建所有 API 请求的起点。 客户端类有两种样式：一种使用 fluent 接口创建请求 (例如，) 另一种接受路径字符串 (`client.Users["user-id"].Manager` 例如 `api("/users/user-id/manager")` ，) 。 当具有请求对象时，可以指定各种选项，如筛选和排序，最后，选择要执行的操作类型。

还有一个[Microsoft Graph PowerShell SDK，](../powershell/get-started.md)它没有任何客户端类。 相反，所有请求都表示为 PowerShell 命令。 例如，若要获取用户的经理，该命令为 `Get-MgUserManager` 。 有关查找 API 调用命令详细信息，请参阅导航[Microsoft Graph PowerShell SDK。](../powershell/navigating.md)

## <a name="read-information-from-microsoft-graph"></a>从 Microsoft Graph

若要从 Microsoft Graph中读取信息，首先需要创建请求对象，然后对请求运行 `GET` 方法。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-read.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a>使用 $select 控制返回的属性

检索实体时，并非所有属性都自动检索;有时需要显式选择它们。 此外，在某些情况下，不需要返回默认属性集。 仅选择所需的属性可以改善请求的性能。 您可以自定义请求以包含 `$select` 包含属性列表的查询参数。

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-select.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a>检索实体列表

检索实体列表与检索单个实体相似，除了有许多用于配置请求的其他选项。 `$filter`查询参数可用于将查询结果集条件匹配的那些行。  `$orderBy`查询参数将请求服务器提供按指定属性排序的实体列表。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-list.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-list.md)]

---

检索实体列表时返回的对象可能是分页集合。 若要详细了解如何获取实体的完整列表，请参阅 [分页浏览集合](../paging.md)。

## <a name="access-an-item-of-a-collection"></a>访问集合的项

对于支持流畅样式的 SDK，可以使用数组索引访问实体集合。 对于基于模板的 SDK，在集合后的路径段中嵌入项标识符就足够了。 对于 PowerShell，标识符作为参数传递。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-index.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a>使用$expand访问相关实体

在请求主实体的同时，可以使用筛选器请求相关实体或 `$expand` 实体集合。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-expand.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a>删除实体

删除请求的构造方式与检索实体的请求相同，但使用请求 `DELETE` 而不是 `GET` 。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-delete.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a>提出 POST 请求以创建新实体

对于支持流畅样式的 SDK，可以使用 方法将新项添加到 `Add` 集合中。 对于基于模板的 SDK，请求对象公开一 `post` 个方法。 对于 `New-*` PowerShell，有一个命令可用于接受映射到要添加的实体的参数。 通常从调用中返回已创建的实体。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-create.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a>使用 PATCH 更新现有实体

Microsoft Graph中的大多数更新都是使用 方法执行的，因此只需在传递的对象中包括要更改 `PATCH` 的属性。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-update.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a>使用 HTTP 标头控制请求行为

可以使用 函数 `Header()` 将自定义标头附加到请求。 对于 PowerShell，仅能通过 方法添加 `Invoke-GraphRequest` 标头。 许多 Microsoft Graph方案使用自定义标头来调整请求的行为。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-headers.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a>提供自定义查询参数

对于支持 Fluent 样式的 SDK，可以使用对象列表提供自定义查询参数 `QueryOptions` 值。 对于基于模板的 SDK，参数经过 URL 编码并添加到请求 URI。 对于 PowerShell 和 Go，为给定 API 定义的查询参数作为参数向相应的命令公开。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-queryparams.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-queryparams.md)]

---
