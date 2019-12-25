---
title: 使用 Microsoft 搜索 API 为数据编制索引
description: 使用 Microsoft Graph 为 Microsoft 搜索服务中的自定义项或外部文件编制索引。
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: f1a39a42f94a072c501c288b55a6b665af0fc640
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870227"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a>使用 Microsoft 搜索 API 为数据编制索引

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可使用 Microsoft Graph 将自定义项或外部文件添加到 [Microsoft 搜索](/microsoftsearch/overview-microsoft-search)体验的搜索结果中。

在无已登录用户的情况下，以应用程序的身份请求为数据编制索引，并使用[包含应用程序权限的访问令牌](/graph/auth-v2-service)进行标识。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a>常见用例

此部分中的 API 用例涉及到构建 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview)，其中包括以下主要步骤：

1. 与外部数据源[建立连接](../api/external-post-connections.md)。
2. [创建并注册架构](../api/externalconnection-post-schema.md)，以描述类型及外部数据的索引编制方式。
3. [编制数据的索引](../api/externalconnection-put-items.md)，将其用作外部项或外部文件。

| 用例                                        | REST 资源                              | 另请参阅 |
|:-------------------------------------------------|:--------------------------------------------|:--|
| **配置操作**                        |                                             |   |
| 建立、更新或删除连接           | [externalConnection](externalconnection.md) | [externalConnection 方法](externalconnection.md#methods) |
| 注册外部数据的架构          | [schema](schema.md)                         | [schema 方法](schema.md#methods) |
| **为操作编制索引**                             |                                             |   |
| 在索引中添加、更新或删除自定义项 | [externalItem](externalitem.md)             | [externalItem 方法](externalItem.md#methods) |
| 在索引中添加、更新或删除文件        | [externalFile](externalfile.md)             | [externalFile 方法](externalfile.md#methods) |

## <a name="known-limitations"></a>已知限制

当前已知的限制如下：

- 组织最多可有 10 个连接。
- 使用 `externalFile` 资源为文件编制索引时不支持自定义属性。
- 仅支持 Azure Active Directory 标识。
- 每秒只能创建 4 个 `externalItem` 或 `externalFile` 资源项。
- 应用程序最多可对一个连接执行 4 个并行操作。
- 连接的容量限制为 70 万个项，或约 70 GB 的数据。
- `externalItem` 或 `externalFile` 实体的最大大小为 4 MB。
- 不支持对结果进行优化和排序。
- 最多可以进行结果排名。

## <a name="next-steps"></a>后续步骤

- 请参阅 [Microsoft 搜索 API 概述](/graph/search-concept-overview)。
- 向下钻取 [externalConnection](externalconnection.md)、[schema](schema.md)、[externalItem](externalitem.md) 和 [externalFile](externalfile.md) 资源的方法、属性和关系。
- 查看 GitHub 中的[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。
