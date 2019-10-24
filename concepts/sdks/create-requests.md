---
title: 使用 Microsoft Graph Sdk 进行 API 调用
description: 提供有关使用 Sdk 创建 Microsoft Graph HTTP 请求的说明。
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: d4fdd5fc6c9a5b2fb0e8acd6d5484176ef179333
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653515"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a>使用 Microsoft Graph Sdk 进行 API 调用

Microsoft Graph SDK 服务库提供了一个客户端类，您可以将其用作创建所有 API 请求的起始点。 有两种类型的客户端类：一种是使用流畅的接口来创建请求（例如`client.Me.Manager`，），另一种是接受路径字符串（例如`api("/me/manager")`）。 当您拥有 request 对象时，可以指定各种选项（如筛选和排序），最后，选择要执行的操作的类型。

## <a name="read-information-from-microsoft-graph"></a>阅读 Microsoft Graph 中的信息

若要从 Microsoft Graph 读取信息，首先需要创建 request 对象，然后对该请求运行`GET`方法。

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]
---

## <a name="use-select-to-control-the-properties-returned"></a>使用 $select 控制返回的属性

检索实体时，并不会自动检索所有属性;有时需要显式选择它们。 此外，在某些情况下，无需返回默认的属性集。 仅选择所需的属性可提高请求的性能。 您可以自定义*request*对象，以使用`$select`属性列表发出查询参数。

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]
---


## <a name="retrieve-a-list-of-entities"></a>检索实体列表

检索实体列表与检索单个实体类似，但有许多其他选项可用于配置请求。 `$filter`查询参数可用于将结果集减少为与提供的条件匹配的那些行。  `$orderBy`查询参数将请求服务器提供按指定属性排序的实体列表。

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]
---

检索实体列表时返回的对象可能是分页的集合。 有关如何获取实体的完整列表的详细信息，请参阅[通过集合进行分页](../paging.md)。

## <a name="access-an-item-of-a-collection"></a>访问集合中的项

对于支持流畅样式的 Sdk，可以使用数组索引访问实体的集合。 对于基于模板的 Sdk，足以将项标识符嵌入到集合后面的路径段中。

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]
---

## <a name="use-expand-to-access-related-entities"></a>使用 $expand 访问相关实体

您可以使用`$expand`筛选器请求与您请求主实体的相关实体或实体集合。  Request `Expand()`对象上的** 函数将添加所需的查询参数。

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]
---


## <a name="delete-an-entity"></a>删除实体

若要删除实体，请采用与检索实体相同的方式构造*请求*。 *Request*对象上的*delete*方法指示要删除实体的愿望。

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]
---

## <a name="make-a-post-request-to-create-a-new-entity"></a>发出 POST 请求以创建新实体

若要在集合中创建新实体，请调用`add`或`post`方法，并传入包含要用于创建新实体的信息的对象。 创建的实体的更新版本通常是从调用返回的。

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]
---

## <a name="updating-an-existing-entity-with-patch"></a>使用修补程序更新现有实体

Microsoft Graph 中的大多数更新都是使用`PATCH`方法执行的，因此只需在传递的对象中包含要更改的属性。  

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]
---


## <a name="use-http-headers-to-control-request-behavior"></a>使用 HTTP 标头控制请求行为

您可以使用`header()`函数将自定义标头附加到请求。 许多 Microsoft Graph 方案使用自定义标头来调整请求的行为。
 
# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]
---

## <a name="provide-custom-query-parameters"></a>提供自定义查询参数

在 API 调用允许自定义查询参数的情况下，可以使用`QueryOptions`对象列表提供这些参数值。

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]
---
