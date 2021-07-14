---
title: Microsoft Graph 中的 Microsoft 搜索 API 概述
description: 使用 Microsoft 搜索 API 来编制内容索引，并将跨 Office 的搜索和编入索引的内容添加到你的应用。
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 061252bb8006cbb3ce195ea656c7dbc50334f66a
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401307"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph"></a>Microsoft Graph 中的 Microsoft 搜索 API 概述

Microsoft 搜索是一种企业搜索引擎，它为组织提高了生产力并提供相关搜索结果。 它控制组织的总体知识和生产力，并显示相关内容，使最终用户了解最新状态。 Microsoft 搜索可以在多种体验中获得，包括 Office、SharePoint、Delve、Windows 和必应。 可使用 Microsoft Graph 中的 Microsoft 搜索 API 将 Microsoft 搜索范围扩展到你的应用。


<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a>为什么使用 Microsoft 搜索 API？

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a>Microsoft 云数据的一个统一搜索终结点

Microsoft 搜索 API 提供一个统一的搜索终结点，让你使用该终结点[查询](/graph/api/search-query) Microsoft 云中的数据（Outlook 邮箱中的邮件和事件）以及 OneDrive 和 SharePoint 中的文件（Microsoft 搜索已编制索引的数据）。

### <a name="include-custom-external-data-in-search-experience-preview"></a>在搜索体验中加入自定义外部数据（预览版）

使用 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview)将 Microsoft 云之外的数据包含在你的搜索体验中。 例如，连接到组织的人力资源数据库或产品目录。 然后使用 Microsoft 搜索 API 无缝[查询](/graph/api/search-query)外部数据源。 

浏览 [Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)以查找随时可用的连接器。 或者，你可以[生成自己的连接器](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases)，为外部自定义项目创建索引并查询特定外部数据源。

### <a name="consistent-up-to-date-search-experience"></a>一致的最新搜索体验

使用 Microsoft 搜索 API 时，客户将获得 Microsoft Graph 所支持的更个性化的相关结果。 你的应用中的搜索体验将返回与 Office 应用程序中的搜索一致的结果。

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a>使用 Microsoft 搜索 API 可以添加或访问哪些数据？

Microsoft 搜索 API 支持在 Microsoft 云中搜索以下内容：

- Outlook 电子邮件[邮件](/graph/api/resources/message)和日历[事件](/graph/api/resources/event)对象
- SharePoint 和 OneDrive 文件和文件夹（[driveItem](/graph/api/resources/driveitem)）， [列表](/graph/api/resources/list)， [listItems](/graph/api/resources/listitem)， [网站](/graph/api/resources/site)和[驱动器](/graph/api/resources/drive)
- 组织中与用户最相关的[人员](/graph/api/resources/person)
- 通过图形连接器平台摄取的内容： [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)（预览版）

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-1.0)（v1.0版本）
- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta)（预览版）
- [使用 Microsoft 搜索 API 索引数据](/graph/api/resources/indexing-api-overview)（预览版）

## <a name="next-steps"></a>后续步骤

- 了解有关 [Microsoft 搜索](/microsoftsearch/)的详细信息。
- 了解有关几个关键用例的详细信息：
  - [管理连接以对外部内容编制索引](connecting-external-content-manage-connections.md)
  - [对外部内容编制索引](connecting-external-content-manage-items.md)
  - [搜索 Outlook 邮件](search-concept-messages.md)
  - [搜索日历事件](search-concept-events.md)
  - [SharePoint 和 OneDrive 中的搜索内容](search-concept-files.md)
  - [搜索外部内容](search-concept-custom-types.md)（预览版）
  - [搜索人员](search-concept-person.md)（预览）
  - [排序搜索结果](search-concept-sort.md)（预览版）
  - [改进搜索结果](search-concept-aggregation.md)（预览版）
  - [请求拼写更正](search-concept-speller.md) （预览版）
  - [搜索显示布局](search-concept-display-layout.md) （预览版）
 
  
- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中探索搜索 API。
- 从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。

## <a name="see-also"></a>另请参阅

- 在 [Microsoft Q&A](/answers/products/m365#microsoft-graph) 上或 GitHub 上与社区互动
