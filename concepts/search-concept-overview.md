---
title: 搜索 API 概述（预览版）
description: 了解如何使用 Microsoft 搜索 API 索引内容，并将跨 Office 的搜索和编入索引的内容添加到应用。
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 4196a2b01576e11f2b9db28a4ea1f89d76f467c5
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955909"
---
# <a name="overview-for-extending-the-microsoft-search-experience-for-apps-on-microsoft-graph-preview"></a>概述在 Microsoft Graph 上扩展应用的 Microsoft 搜索体验（预览版）

Microsoft 搜索是一种企业搜索引擎，它为组织提高了生产力并提供相关搜索结果。 它控制组织的总体知识和生产力，并显示相关内容，使最终用户了解最新状态。 Microsoft 搜索可以在多种体验中获得，包括 Office、SharePoint、Delve、Windows 和必应。 Microsoft 搜索 API 允许应用为其应用客户扩展类似的搜索体验。 

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a>为什么使用 Microsoft 搜索 API？

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a>Microsoft 云数据的一个统一搜索终结点

Microsoft Search API 提供一个统一的搜索终结点，让开发人员[查询](/graph/api/search-query?view=graph-rest-beta) Microsoft 云中的数据（Outlook 邮箱中的邮件和事件），以及 OneDrive 和 SharePoint 中的文件（Microsoft 搜索已索引的数据）。

### <a name="include-custom-external-data-in-search-experience"></a>在搜索体验中包括自定义外部数据

希望在其搜索体验中包括 Microsoft 云之外的数据的客户可以使用[连接器](/microsoftsearch/connectors-overview)连接到特定数据源（如组织的人力资源数据库或产品目录），并使用 Microsoft 索引 API 无缝[查询](/graph/api/search-query?view=graph-rest-beta)外部数据源。 [Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)列出了大量随时可用的连接器。 或者，客户可以[构建连接器](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases)、索引外部自定义项目和文件以及查询特定外部数据源。

### <a name="consistent-up-to-date-search-experience"></a>一致的最新搜索体验

使用 Microsoft 搜索 API，客户可从获得 Microsoft Graph 所支持的更多个性化相关结果中受益。 这也会使应用中的搜索返回与 Office 应用程序中的搜索一致的结果。

## <a name="what-data-can-i-add-or-access-by-using-these-apis"></a>使用这些 API 可以添加或访问哪些数据？

Microsoft 搜索支持在 Microsoft 云中搜索内容：

- Outlook [message](/graph/api/resources/message?view=graph-rest-beta) 和 [event](/graph/api/resources/event?view=graph-rest-beta) 对象
- SharePoint 和 OneDrive [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 文件对象

此外，还可对外部内容编制索引和搜索：

- 自定义类型的 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) 对象
- 众所周知类型的 [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) 对象

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta)
- [使用 Microsoft 搜索 API 为数据编制索引](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>后续步骤

- 了解有关 [Microsoft 搜索](/microsoftsearch/)的详细信息。
- 了解有关几个关键用例的详细信息：
  - [搜索 Outlook 邮件](search-concept-messages.md)
  - [搜索日历事件](search-concept-events.md)
  - [管理连接以对外部内容编制索引](search-index-manage-connections.md)
  - [对外部内容编制索引](search-index-manage-items.md)
  - [搜索自定义类型 (externalItem)](search-concept-custom-types.md)
  - [搜索文件（包括 externalFile）](search-concept-files.md)
- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中探索搜索 API。
- 从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。

## <a name="see-also"></a>另请参阅

与社区互动：

- [在 StackOverflow 上讨论](https://stackoverflow.com/questions/tagged/microsoft-graph-search)
