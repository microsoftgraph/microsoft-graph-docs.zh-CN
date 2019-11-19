---
title: 使用 Microsoft 搜索 API 为数据编制索引
description: 借助 Microsoft Graph，应用可以为 Microsoft 搜索服务中的自定义项或外部文件编制索引。
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: e6afa7be0f1bf7dbda0561f8bd0e89ce8b0a3e4d
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703782"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a>使用 Microsoft 搜索 API 为数据编制索引

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

借助 Microsoft Graph，应用可以将自定义项或外部文件添加到 [Microsoft 搜索](/microsoftsearch/overview-microsoft-search)体验的搜索结果中。

在无已登录用户的情况下，以应用程序的身份请求为数据编制索引，并使用[包含应用程序权限的访问令牌](/graph/auth-v2-service)进行标识。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a>常见用例

此部分中的 API 用例以生成 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview)为中心，其中涉及以下方面的主要步骤：

1. 与外部数据源[建立连接](../api/external-post-connections.md)
2. [创建并注册架构](../api/externalconnection-post-schema.md)，以描述类型以及如何为外部数据编制索引
3. [为数据编制索引](../api/externalconnection-put-items.md)作为外部项或外部文件

| 用例                                        | REST 资源                              | 另请参阅 |
|:-------------------------------------------------|:--------------------------------------------|:--|
| **配置操作**                        |                                             |   |
| 建立、更新或删除连接           | [externalConnection](externalconnection.md) | [externalConnection 的方法](externalconnection.md#methods) |
| 注册外部数据的架构          | [schema](schema.md)                         | [schema 的方法](schema.md#methods) |
| **为操作编制索引**                             |                                             |   |
| 在索引中添加、更新或删除自定义项 | [externalItem](externalitem.md)             | [externalItem 的方法](externalItem.md#methods) |
| 在索引中添加、更新或删除文件        | [externalFile](externalfile.md)             | [externalFile 的方法](externalfile.md#methods) |

## <a name="known-limitations"></a>已知限制

在预览期间，请注意以下限制。

- 组织最多可有 10 个连接。
- 使用 `externalFile` 资源为文件编制索引时，不支持自定义属性。
- 仅支持 Azure Active Directory 标识。
- 创建 `externalItem` 或 `externalFile` 资源时，每秒的上限为 4 个项。
- 应用程序最多可对连接执行 4 个并行操作。
- 连接的容量限制为 70 万个项，或约 70 GB 的数据。
- `externalItem` 或 `externalFile` 实体的最大大小为 4 MB。
- 不支持对结果进行优化和排序。
- 最多可以进行结果排名。

## <a name="next-steps"></a>后续步骤

- [Microsoft 搜索 API 概述](/graph/search-concept-overview)
- 向下钻取 [externalConnection](externalconnection.md)、[schema](schema.md)、[externalItem](externalitem.md) 和 [externalFile](externalfile.md) 资源的方法、属性和关系。
- 查看 GitHub 中的[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。
