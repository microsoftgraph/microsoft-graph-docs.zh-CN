---
title: Microsoft Graph 连接器 API 限制
description: 设计 Microsoft Graph 连接器时，请牢记实施和运行限制。 包括连接、架构和组限制。
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 517d5f2d62e3d9025b8492433af2ec3fc0bd69a3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094233"
---
# <a name="microsoft-graph-connectors-api-limits"></a>Microsoft Graph 连接器 API 限制

本文介绍 Microsoft Graph 连接器的实施和运行限制。 设计连接器时，请牢记这些限制。

## <a name="connection-limits"></a>连接限制

| 限制类型 | 限制 |
| ---------- | ----- |
| 每个 Microsoft 365 租户的[连接](/graph/api/resources/externalconnectors-externalconnection)资源 | 10 |
| 每个连接的[项目数](/graph/api/resources/externalconnectors-externalitem) | 700,000 项 |
| 连接字节大小 | 70 GB |

## <a name="schema-limits"></a>架构限制

| 限制类型 | 限制 |
| ---------- | ----- |
| 可以在[架构](/graph/api/resources/externalconnectors-schema)中定义属性，描述通过连接引入的数据。 | 128 |

## <a name="group-limits"></a>组限制

| 限制类型 | 限制 |
| ---------- | ----- |
| 每个 Microsoft 365 租户的[外部组](/graph/api/resources/externalconnectors-externalgroup) | 100,000 | 
| 组管理[限制](#throttling)阈值中每秒允许的请求数（请求数/秒）。 | 1,000 |

## <a name="item-ingestion"></a>项引入

| 限制类型 | 限制 |
| ---------- | ----- |
| 通过连接引入项目的吞吐量限制。 | 每秒 4 个项目 <br> 每小时 250 MB |
| 项目大小；此限制适用于[引入项目并为其建立索引](/graph/api/externalconnectors-externalconnection-put-items)时的请求正文。 | 4 MB |
| 属性大小 | 不适用 |

## <a name="throttling"></a>限制

当超过 [限制](throttling.md) 阈值时，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），并且请求失败。在失败请求的响应标头中会返回建议的等待时间。

限制行为可能取决于请求的类型和数量。例如，如果具有大量请求，则会限制所有请求类型。阈值限制因请求类型而异。因此，你可能会遇到写入受到限制，但仍允许读取的情况。
