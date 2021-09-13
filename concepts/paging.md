---
title: '在应用中对 Microsoft Graph 数据进行分页 '
description: '响应中的 odata.nextLink` 属性，其中包含下一页结果的 URL。 '
author: davidmu1
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 8bfa1bb87e5a05e82d65e75742be4c9d6761c183
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59071719"
---
# <a name="paging-microsoft-graph-data-in-your-app"></a>在应用中对 Microsoft Graph 数据进行分页 

由于服务器端分页或由于使用 `$top` 查询参数来明确限制请求中的页面大小，致使针对 Microsoft Graph 的一些查询返回多页数据。当结果集跨多个页面时，Microsoft Graph 将在响应中返回 `@odata.nextLink` 属性，该属性包含指向结果下一页的 URL。 

例如，以下 URL 要求对组织中的所有用户使用页面大小 5（使用 `$top` 查询参数指定）：

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

如果结果包含超过 5 个用户，则 Microsoft Graph 将返回一个下列类似的 `@odata.nextLink` 属性以及第一页的用户。

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

可以通过将 `@odata.nextLink` 属性的 URL 值发送到 Microsoft Graph 来检索结果的下一页。 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

Microsoft Graph 将继续通过每次响应返回对 `@odata.nextLink` 属性中下一页数据的引用，直到读取结果的所有页面。

>**重要说明：** 应该在请求的 `@odata.nextLink` 属性中包括整个 URL，以获取下一页结果。 根据正在对其执行查询的 API， `@odata.nextLink` URL 值将包含 `$skiptoken` 或 `$skip` 查询参数。 该 URL 还包含原始请求中存在的所有其他查询参数。 请勿尝试提取 `$skiptoken` 或 `$skip` 值，也不要在不同的请求中使用它。 

分页行为因 Microsoft Graph API 不同而异。 处理分页数据时，应考虑以下几点：

- 不同的 API 可能具有不同的默认页面大小和最大页面大小。
- 如果指定超过相应 API 最大页面大小的页面大小（通过 `$top` 查询参数），则不同 API 的行为会有所不同。 具体取决于 API，所请求的页面大小可能会被忽略，它默认选择相应 API 的最大页面大小，否则 Microsoft Graph 会返回错误。 
- 并不是所有的资源和关系都支持分页。例如，针对 [directoryRoles](/graph/api/resources/directoryrole) 的查询不支持分页。这包括读取角色对象本身以及角色成员。
- 对目录资源进行分页时，默认情况下，后续页面请求中不包含任何其他请求标头(如 **ConsistencyLevel** 标头)。 如果需要在后续请求中发送这些标头，则必须显式设置它们。
- 在针对目录资源进行查询时使用 `$count=true` 查询字符串时， `@odata.count` 属性将仅出现在分页数据的第一页中。

## <a name="learn-more-about-paging"></a>详细了解分页
以下视频介绍了 Microsoft Graph 中的分页。

> [!VIDEO https://www.youtube-nocookie.com/embed/DB_NoC9a1JI]
