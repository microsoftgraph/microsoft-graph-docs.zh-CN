---
title: 使用 Microsoft 搜索 API 为数据编制索引
description: 使用 Microsoft Graph 为 Microsoft 搜索服务中的自定义项编制索引。
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 69a1c99af429b93d7fbddbea4e76523b281541d7
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366961"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a>使用 Microsoft 搜索 API 为数据编制索引

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可使用 Microsoft Graph 将自定义项添加到 [Microsoft 搜索](/microsoftsearch/overview-microsoft-search)体验的搜索结果中。

在无已登录用户的情况下，以应用程序的身份请求为数据编制索引，并使用[包含应用程序权限的访问令牌](/graph/auth-v2-service)进行标识。

## <a name="common-use-cases"></a>常见用例

此部分中的 API 用例涉及到构建 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview)，其中包括以下主要步骤：

1. 与外部数据源[建立连接](../api/external-post-connections.md)。
2. [创建并注册架构](../api/externalconnection-post-schema.md)，以描述类型及外部数据的索引编制方式。
3. 将数据作为外部项[编制索引](../api/externalconnection-put-items.md)。

| 用例                                        | REST 资源                              | 另请参阅 |
|:-------------------------------------------------|:--------------------------------------------|:--|
| **配置操作**                        |                                             |   |
| 建立、更新或删除连接           | [externalConnection](externalconnection.md) | [externalConnection 方法](externalconnection.md#methods) |
| 注册外部数据的架构          | [schema](schema.md)                         | [schema 方法](schema.md#methods) |
| **为操作编制索引**                             |                                             |   |
| 在索引中添加、更新或删除自定义项 | [externalItem](externalitem.md)             | [externalItem 方法](externalItem.md#methods) |

## <a name="known-limitations"></a>已知限制

当前已知的限制如下：

- 组织最多可有 10 个连接。
- 仅支持 Azure Active Directory 标识。
- 每秒只能创建 4 个 `externalItem` 资源项。
- 应用程序最多可对一个连接执行 4 个并行操作。
- 连接的容量限制为 70 万个项，或约 70 GB 的数据。
- `externalItem` 实体的最大大小为 4 MB。
- 不支持对结果进行排序。
- 最多可以进行结果排名。

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤

- 请参阅 [Microsoft 搜索 API 概述](/graph/search-concept-overview)。
- 向下钻取 [externalConnection](externalconnection.md)、[schema](schema.md) 和[externalItem](externalitem.md) 资源的方法、属性和关系。
- 查看 GitHub 中的[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。


