---
title: Microsoft Graph 中的 Microsoft 搜索 API 概述（预览版）
description: 使用 Microsoft 搜索 API 来编制内容索引，并将跨 Office 的搜索和编入索引的内容添加到你的应用。
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: d4c16bd0175f8ae0cd9d8e03f549bea9eff3db63
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373501"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph-preview"></a>Microsoft Graph 中的 Microsoft 搜索 API 概述（预览版）

Microsoft 搜索是一种企业搜索引擎，它为组织提高了生产力并提供相关搜索结果。 它控制组织的总体知识和生产力，并显示相关内容，使最终用户了解最新状态。 Microsoft 搜索可以在多种体验中获得，包括 Office、SharePoint、Delve、Windows 和必应。 可使用 Microsoft Graph 中的 Microsoft 搜索 API 将 Microsoft 搜索范围扩展到你的应用。

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a>为什么使用 Microsoft 搜索 API？

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a>Microsoft 云数据的一个统一搜索终结点

Microsoft 搜索 API 提供一个统一的搜索终结点，让你使用该终结点[查询](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) Microsoft 云中的数据（Outlook 邮箱中的邮件和事件）以及 OneDrive 和 SharePoint 中的文件（Microsoft 搜索已编制索引的数据）。

### <a name="include-custom-external-data-in-search-experience"></a>在搜索体验中包括自定义外部数据

希望在其搜索体验中包括 Microsoft 云之外的数据的客户可以使用[连接器](/microsoftsearch/connectors-overview)连接到特定数据源（如组织的人力资源数据库或产品目录），并使用 Microsoft 索引 API 无缝[查询](/graph/api/search-query?view=graph-rest-beta&preserve-view=true)外部数据源。 [Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)列出了大量随时可用的连接器。 或者，客户可以[生成连接器](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases)、为外部自定义项编制索引，并能查询特定外部数据源。

### <a name="consistent-up-to-date-search-experience"></a>一致的最新搜索体验

使用 Microsoft 搜索 API 时，客户将获得 Microsoft Graph 所支持的更个性化的相关结果。 你的应用中的搜索体验将返回与 Office 应用程序中的搜索一致的结果。

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a>使用 Microsoft 搜索 API 可以添加或访问哪些数据？

Microsoft 搜索 API 支持在 Microsoft 云中搜索以下内容：

- Outlook 电子邮件[邮件](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true)和日历[事件](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true)对象
- SharePoint 和 OneDrive 文件和文件夹（[driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)）， [列表](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true)， [listItems](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true)， [网站](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true)和[驱动器](/graph/api/resources/drive?view=graph-rest-beta&preserve-view=true)
- 通过图形连接器平台摄取的内容： [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
- [使用 Microsoft 搜索 API 为数据编制索引](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>后续步骤

- 了解有关 [Microsoft 搜索](/microsoftsearch/)的详细信息。
- 了解有关几个关键用例的详细信息：
  - [管理连接以对外部内容编制索引](search-index-manage-connections.md)
  - [对外部内容编制索引](search-index-manage-items.md)
  - [搜索 Outlook 邮件](search-concept-messages.md)
  - [搜索日历事件](search-concept-events.md)
  - [SharePoint 和 OneDrive 中的搜索内容](search-concept-files.md)
  - [搜索外部联系人](search-concept-custom-types.md)
  - [排序搜索结果](search-concept-sort.md)
  - [改进搜索结果](search-concept-aggregation.md)
  
- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中探索搜索 API。
- 从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。

## <a name="see-also"></a>另请参阅

- 在 [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) 或 GitHub 上与社区互动。
