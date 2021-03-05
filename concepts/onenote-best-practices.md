---
title: 使用 Microsoft Graph 中的 OneNote API 的最佳做法
description: 本文提供了有关使用 Microsoft Graph 中的 OneNote API 的建议。 这些建议基于 Microsoft Q&A 和 Twitter 上的常见问题解答。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 8ceb848e4d48954d9a08c8bc9f7b28e2521c9aed
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472802"
---
# <a name="best-practices-for-working-with-the-onenote-api-in-microsoft-graph"></a>使用 Microsoft Graph 中的 OneNote API 的最佳做法

本文提供了有关使用 Microsoft Graph 中的 OneNote API 的建议。 这些建议基于 Microsoft Q&A [和](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)  Twitter 上的常见问题解答。

## <a name="use-select-to-select-the-minimum-set-of-properties-you-need"></a>使用 $select 选择所需的最小属性集

查询资源（例如，笔记本中的分区）时，会发出类似于以下内容的请求。

```http
GET ~/notebooks/{id}/sections
```

这将检索分区的所有属性。 然而，你可能并不需要所有属性。 可以使用 `$select` 查询参数只返回所需属性，如下面的示例中所示。

```http
GET ~/notebooks/{id}/sections?$select=id,displayName
```

同样的方法适用于其他 OneNote API。

## <a name="use-expand-instead-of-making-multiple-api-calls"></a>使用 $expand 而不是进行多个 API 调用

假定你要在分层视图中检索用户的所有笔记本、分区和分区组。 可以通过执行以下操作来实现：

* 调用 `GET ~/notebooks` 以获取笔记本的列表。

* 对于每个检索的笔记本，调用 `GET ~/notebooks/{notebookId}/sections` 以检索分区的列表。

* 对于每个检索的笔记本，调用 `GET ~/notebooks/{notebookId}/sectionGroups` 以检索分区组的列表。

* （可选）以递归方式遍历分区组。

虽然此方法有效（同时有一些到服务的额外顺序往返），但更好的方法是使用 `$expand` 查询参数。 

```http
GET ~/notebooks?$expand=sections,sectionGroups($expand=sections)
```

这将在一个网络往返中产生同样的结果，而且性能更佳。

## <a name="when-getting-all-pages-for-a-user-do-so-for-each-section-separately"></a>获取用户的所有页面时，分别对每个分区执行此操作

当 Microsoft Graph 公开一个终结点来检索所有页面时，这并不是获取用户可以访问的所有页面的最佳方式。 如果用户拥有的分区过多，可能会导致超时或性能降低。 最好遍历每个分区，从而分别获取每个分区的页面。

例如，不使用此调用（此 API 已分页，因此无法一次获取所有页面）：

```http
GET ~/pages
```

最好多次使用以下调用（特别是在你不需要所有分区的情况下）：

```http
GET ~/sections/{id}/pages
```

获取页面元数据时，请覆盖默认的 `lastModifiedDateTime` 排序。 当不必按 `lastModifiedDateTime` 对页面进行排序时，获取页面的速度更快。 为此，可以按任何其他属性进行排序；例如：

```http
GET ~/sections/{id}/pages?$select=id,title,createdDateTime&$orderby=createdDateTime
```
