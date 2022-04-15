---
title: 使用 Microsoft Graph SDK 进行 API 调用
description: 提供有关使用 SDK 创建 Microsoft Graph HTTP 请求的说明。
ms.localizationpriority: medium
author: DarrelMiller
ms.openlocfilehash: 49be5a3fdb2ead7e8e3a4d39b459b7ef068a9a74
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848690"
---
<!-- markdownlint-disable MD025 -->

# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a>使用 Microsoft Graph SDK 进行 API 调用

Microsoft Graph SDK 服务库提供一个客户端类，你可以使用该类作为创建所有 API 请求的起点。 客户端类有两种样式：一种使用 Fluent 接口创建请求 (例如， `client.Users["user-id"].Manager`) ，另一种接受路径字符串 (例如 `api("/users/user-id/manager")` ，) 。 拥有请求对象时，可以指定各种选项，例如筛选和排序，最后选择要执行的操作类型。

还有 [Microsoft Graph PowerShell SDK](/powershell/microsoftgraph/get-started.md)，它根本没有客户端类。 相反，所有请求都表示为 PowerShell 命令。 例如，若要获取用户的管理器，命令为 `Get-MgUserManager`。 有关查找 API 调用命令的详细信息，请参[阅导航 Microsoft Graph PowerShell SDK](/powershell/microsoftgraph/navigating.md)。

## <a name="read-information-from-microsoft-graph"></a>从 Microsoft Graph读取信息

若要从 Microsoft Graph 读取信息，首先需要创建请求对象，然后对请求运行`GET`该方法。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-read.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a>使用$select控制返回的属性

检索实体时，并非所有属性都会自动检索;有时需要显式选择它们。 此外，在某些情况下，不需要返回默认属性集。 仅选择所需的属性可以提高请求的性能。 可以自定义请求，以包含 `$select` 包含属性列表的查询参数。

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-select.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a>检索实体列表

检索实体列表类似于检索单个实体，但用于配置请求的其他许多选项除外。 查询 `$filter` 参数可用于将结果集减少到仅与提供的条件匹配的行。  查询 `$orderBy` 参数将请求服务器提供按指定属性排序的实体列表。

[!INCLUDE [aad-advanced-queries-note](../../includes/aad-advanced-queries-note.md)]

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-list.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-list.md)]

---

检索实体列表时返回的对象可能是分页集合。 有关如何获取实体完整列表的详细信息，请参阅 [通过集合进行分页](../paging.md)。

## <a name="access-an-item-of-a-collection"></a>访问集合的项

对于支持流式样式的 SDK，可以使用数组索引访问实体集合。 对于基于模板的 SDK，足以在集合后的路径段中嵌入项标识符。 对于 PowerShell，标识符作为参数传递。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-index.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a>使用$expand访问相关实体

在请求主实体的同时，可以使用 `$expand` 筛选器请求相关实体或实体集合。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-expand.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a>删除实体

删除请求的构造方式与检索实体的请求相同，但使用 `DELETE` 请求而不是 `GET`请求。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-delete.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a>发出 POST 请求以创建新实体

对于支持流式样式的 SDK，可以使用 `Add` 方法将新项添加到集合中。 对于基于模板的 SDK，请求对象会公开一种方法 `post` 。 对于 PowerShell，可以使用一个 `New-*` 命令来接受映射到要添加的实体的参数。 创建的实体通常从调用返回。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-create.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a>使用 PATCH 更新现有实体

Microsoft Graph中的大多数更新都是使用方法`PATCH`执行的，因此只需在传递的对象中包含要更改的属性。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-update.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a>使用 HTTP 标头控制请求行为

可以使用函数 `Header()` 将自定义标头附加到请求。 对于 PowerShell，仅可通过 `Invoke-GraphRequest` 该方法添加标头。 许多 Microsoft Graph方案使用自定义标头来调整请求的行为。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-headers.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a>提供自定义查询参数

对于支持流式样式的 SDK，可以使用对象列表 `QueryOptions` 提供自定义查询参数值。 对于基于模板的 SDK，参数是 URL 编码的，并添加到请求 URI 中。 对于 PowerShell 和 Go，给定 API 的定义查询参数将作为参数公开给相应的命令。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-queryparams.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-queryparams.md)]

---
