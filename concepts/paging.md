---
title: '在应用中对 Microsoft Graph 数据进行分页 '
description: '响应中的 odata.nextLink` 属性，其中包含下一页结果的 URL。 '
author: piotrci
ms.openlocfilehash: b5c6c6adafde4d1cce4135af1b1bb23d068aab27
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348942"
---
# <a name="paging-microsoft-graph-data-in-your-app"></a>在应用中对 Microsoft Graph 数据进行分页 

由于服务器端分页或由于使用 `$top` 查询参数来明确限制请求中的页面大小，致使针对 Microsoft Graph 的一些查询返回多页数据。当结果集跨多个页面时，Microsoft Graph 将在响应中返回 `@odata.nextLink` 属性，该属性包含指向结果下一页的 URL。 

例如，以下 URL 要求对组织中的所有用户使用页面大小 5（使用 `$top` 查询参数指定）：

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

如果结果包含超过 5 个用户，则 Microsoft Graph 将返回一个下列类似的 `@odata:nextLink` 属性以及第一页的用户。

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

可以通过将 `@odata:nextLink` 属性的 URL 值发送到 Microsoft Graph 来检索结果的下一页。 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

Microsoft Graph 将继续通过每次响应返回对 `@odata:nextLink` 属性中下一页数据的引用，直到读取结果的所有页面。

>**重要说明：** 应该在请求的 `@odata:nextLink` 属性中包括整个 URL，以获取下一页结果。 根据正在对其执行查询的 API， `@odata:nextLink` URL 值将包含 `$skiptoken` 或 `$skip` 查询参数。 该 URL 还包含原始请求中存在的所有其他查询参数。 请勿尝试提取 `$skiptoken` 或 `$skip` 值，也不要在不同的请求中使用它。 

分页行为因 Microsoft Graph API 不同而异。 处理分页数据时，应考虑以下几点：

- 不同的 API 可能具有不同的默认页面大小和最大页面大小。
- 如果指定超过相应 API 最大页面大小的页面大小（通过 `$top` 查询参数），则不同 API 的行为会有所不同。 具体取决于 API，所请求的页面大小可能会被忽略，它默认选择相应 API 的最大页面大小，否则 Microsoft Graph 会返回错误。 
- 并不是所有的资源和关系都支持分页。例如，针对 [directoryRoles](/graph/api/resources/directoryrole?view=graph-rest-1.0) 的查询不支持分页。这包括读取角色对象本身以及角色成员。
