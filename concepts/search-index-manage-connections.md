---
title: 创建、更新和删除与 Microsoft 搜索服务的连接
description: 了解如何使用 Microsoft Graph 管理与 Microsoft 搜索服务的连接
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 99f0ab4591caa6c311f2771f1c6a0772a8f16087
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892798"
---
# <a name="create-update-and-delete-connections-to-the-microsoft-search-service"></a>创建、更新和删除与 Microsoft 搜索服务的连接

外部服务与 Microsoft 搜索服务的连接由 Microsoft Graph 中的 [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) 资源表示。

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

通过连接，你的应用程序可以为要编入索引的项目[定义架构](/graph/api/externalconnection-post-schema?view=graph-rest-beta)，并为服务提供终结点，以便[在索引中添加、更新或删除项目](search-index-manage-items.md)。 创建连接是应用程序将项目添加到搜索索引的第一步。

## <a name="create-a-connection"></a>创建连接

应用程序必须先按照以下步骤创建并配置连接，才能将项目添加到搜索索引。

- 使用唯一 ID、显示名称和说明[创建连接](/graph/api/external-post-connections?view=graph-rest-beta)。
- [注册架构](/graph/api/externalconnection-post-schema?view=graph-rest-beta)，以定义索引中将包含的字段。

> [!IMPORTANT]
> 架构注册后，不能为现有连接更改架构。

## <a name="update-a-connection"></a>更新连接

可通过[更新连接](/graph/api/externalconnection-update?view=graph-rest-beta)来更改现有连接的显示名称或说明。

## <a name="delete-a-connection"></a>删除连接

可[删除连接](/graph/api/externalconnection-delete?view=graph-rest-beta)，并删除通过该连接进行索引的所有项目。

## <a name="next-steps"></a>后续步骤

- [为什么使用 Microsoft 搜索 API？](search-concept-overview.md#why-use-the-microsoft-search-api)
- [查看索引 API 参考](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [Microsoft Graph 连接器概述](/microsoftsearch/connectors-overview)
- 从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)
