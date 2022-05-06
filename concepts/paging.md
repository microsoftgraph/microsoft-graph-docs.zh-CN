---
title: '在应用中对 Microsoft Graph 数据进行分页 '
description: '响应中的 odata.nextLink` 属性，其中包含下一页结果的 URL。 '
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 82d891298a3c33b0bb496c5ad8a1475ecd295934
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208860"
---
# <a name="paging-microsoft-graph-data-in-your-app"></a>在应用中对 Microsoft Graph 数据进行分页 

由于服务器端分页或由于使用 `$top` 查询参数来明确限制请求中的页面大小，针对 Microsoft Graph 的一些查询返回了多页数据。当需要多个查询请求以检索全部结果时，Microsoft Graph 将在响应中返回包含指向执行下一结果页面的 URL 的 `@odata.nextLink` 属性。 

例如，以下 URL 要求对组织中的所有用户使用页面大小 5（使用 `$top` 查询参数指定）：

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

如果该结果包含更多结果，则 Microsoft Graph 将返回类似于以下的 `@odata.nextLink` 属性以及结果首页：

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

可以通过将 `@odata.nextLink` 属性的 URL 值发送到 Microsoft Graph 来检索结果的下一页。 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

在读取结果的所有页面之前，Microsoft Graph 将继续通过每次响应返回对 `@odata.nextLink` 属性中下一页结果的引用。 要读取所有结果，必须继续使用每个响应中返回的 `@odata.nextLink` 属性打开 Microsoft Graph，直到不再返回 `@odata.nextLink` 属性。

>**重要说明：** 应该在请求的 `@odata.nextLink` 属性中包括整个 URL，以获取下一页结果。 根据正在对其执行查询的 API， `@odata.nextLink` URL 值将包含 `$skiptoken` 或 `$skip` 查询参数。 该 URL 还包含原始请求中存在的所有其他查询参数。 请勿尝试提取 `$skiptoken` 或 `$skip` 值，也不要在不同的请求中使用它。 

分页行为因 Microsoft Graph API 不同而异。 处理分页数据时，应考虑以下几点：

- 结果页可能包含零个或多个结果。
- 不同的 API 可能具有不同的默认页面大小和最大页面大小。
- 如果指定超过相应 API 最大页面大小的页面大小（通过 `$top` 查询参数），则不同 API 的行为会有所不同。 具体取决于 API，所请求的页面大小可能会被忽略，它默认选择相应 API 的最大页面大小，否则 Microsoft Graph 会返回错误。 
- 并不是所有的资源和关系都支持分页。例如，针对 [directoryRoles](/graph/api/resources/directoryrole) 的查询不支持分页。这包括读取角色对象本身以及角色成员。
- 对目录资源进行分页时，默认情况下，后续页面请求中不包含任何其他请求标头(如 **ConsistencyLevel** 标头)。 如果需要在后续请求中发送这些标头，则必须显式设置它们。
- 在针对目录资源进行查询时使用 `$count=true` 查询字符串时， `@odata.count` 属性将仅出现在分页数据的第一页中。

## <a name="learn-more-about-paging"></a>详细了解分页
以下视频介绍了 Microsoft Graph 中的分页。

> [!VIDEO https://www.youtube-nocookie.com/embed/DB_NoC9a1JI]
