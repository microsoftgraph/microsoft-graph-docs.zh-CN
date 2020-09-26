---
title: 使用 Microsoft Graph Sdk 进行 API 调用
description: 提供有关使用 Sdk 创建 Microsoft Graph HTTP 请求的说明。
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 1338cbe7411a3643eaa5c1e1e58cf8d5b9b47c0a
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288281"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a>使用 Microsoft Graph Sdk 进行 API 调用

Microsoft Graph SDK 服务库提供了一个客户端类，您可以将其用作创建所有 API 请求的起始点。 有两种类型的客户端类：一种是使用流畅的接口来创建请求 (例如， `client.Users["user-id"].Manager`) ，另一种是接受路径字符串 (例如， `api("/users/user-id/manager")`) 。 当您拥有 request 对象时，可以指定各种选项（如筛选和排序），最后，选择要执行的操作的类型。

还有 [Microsoft Graph POWERSHELL SDK](../powershell/get-started.md)，它根本没有客户端类。 相反，所有请求都表示为 PowerShell 命令。 例如，若要获取用户的经理，该命令是 `Get-MgUserManager` 。 有关查找有关 API 调用的命令的详细信息，请参阅 [导航 Microsoft Graph POWERSHELL SDK](../powershell/navigating.md)。

## <a name="read-information-from-microsoft-graph"></a>阅读 Microsoft Graph 中的信息

若要从 Microsoft Graph 读取信息，首先需要创建 request 对象，然后 `GET` 对该请求运行方法。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-read.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a>使用 $select 控制返回的属性

检索实体时，并不会自动检索所有属性;有时需要显式选择它们。 此外，在某些情况下，无需返回默认的属性集。 仅选择所需的属性可提高请求的性能。 您可以自定义请求，以将 `$select` 查询参数包含在属性列表中。

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-select.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a>检索实体列表

检索实体列表与检索单个实体类似，但有许多其他选项可用于配置请求。 `$filter`查询参数可用于将结果集减少为与提供的条件匹配的那些行。  `$orderBy`查询参数将请求服务器提供按指定属性排序的实体列表。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-list.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

---

检索实体列表时返回的对象可能是分页的集合。 有关如何获取实体的完整列表的详细信息，请参阅 [通过集合进行分页](../paging.md)。

## <a name="access-an-item-of-a-collection"></a>访问集合中的项

对于支持流畅样式的 Sdk，可以使用数组索引访问实体的集合。 对于基于模板的 Sdk，足以将项标识符嵌入到集合后面的路径段中。 对于 PowerShell，标识符作为参数传递。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-index.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a>使用 $expand 访问相关实体

您可以使用 `$expand` 筛选器请求与您请求主实体的相关实体或实体集合。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-expand.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a>删除实体

删除请求的构造方式与检索实体的请求相同，但使用的 `DELETE` 是请求而不是 `GET` 。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-delete.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a>发出 POST 请求以创建新实体

对于支持流畅样式的 Sdk，可以使用方法将新项目添加到集合中 `Add` 。 对于基于模板的 Sdk，request 对象公开了一个 `post` 方法。 对于 PowerShell， `New-*` 可以使用可接受映射到要添加的实体的参数的命令。 创建的实体通常是从调用返回的。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-create.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a>使用修补程序更新现有实体

Microsoft Graph 中的大多数更新都是使用 `PATCH` 方法执行的，因此只需在传递的对象中包含要更改的属性。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-update.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a>使用 HTTP 标头控制请求行为

您可以使用 `Header()` 函数将自定义标头附加到请求。 对于 PowerShell，仅在使用方法时才可以添加标头 `Invoke-GraphRequest` 。 许多 Microsoft Graph 方案使用自定义标头来调整请求的行为。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-headers.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a>提供自定义查询参数

对于支持流畅样式的 Sdk，可以使用对象列表提供自定义查询参数值 `QueryOptions` 。 对于基于模板的 Sdk，参数是 URL 编码的，并添加到请求 URI。 对于 PowerShell，为给定 API 定义的查询参数作为参数公开给相应的命令。

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-queryparams.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

---
