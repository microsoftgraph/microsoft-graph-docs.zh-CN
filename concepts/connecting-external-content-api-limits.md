---
title: Microsoft Graph 连接器 API 限制
description: Microsoft Graph 连接器的实施和运行限制。
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 88cd4d08db4b903e188c82dd38c8d5b89131887f
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247334"
---
# <a name="microsoft-graph-connectors-api-limits"></a>Microsoft Graph 连接器 API 限制

本文介绍 Microsoft Graph 连接器的实施和运行限制。 设计连接器时，请牢记这些限制。

## <a name="connection-limits"></a>连接限制

| **限制** | **说明** |
| --------- | --------------- |
| **10 个连接** | 每个 Microsoft 365 租户的最大[连接](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-1.0&preserve-view=true)资源数。 |
| **700,000 项** | 每个连接的最大[项目](/graph/api/resources/externalconnectors-externalitem?view=graph-rest-1.0&preserve-view=true)数。 |
| **70 GB** | 连接的最大字节大小。 |

## <a name="schema-limits"></a>架构限制

| **限制** | **说明** |
| --------- | --------------- |
| **128 个属性** | 可以在[架构](/graph/api/resources/externalconnectors-schema?view=graph-rest-1.0&preserve-view=true)中定义的最大数量的属性，描述通过连接引入的数据。 |

## <a name="group-limits"></a>组限制

| **限制** | **说明** |
| --------- | --------------- |
| **100,000** | 每个 Microsoft 365 租户的最大[外部组](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true)数量。 |
| **1000 个请求/秒** | 组管理[限制](#throttling)阈值中每秒允许的最大请求数。 |

## <a name="item-ingestion"></a>项引入

| **限制** | **说明** |
| --------- | --------------- |
| **每秒 4 个项目（每小时 250 MB）** | 通过连接引入项目的吞吐量限制。 |
| **4 MB** | 项目的最大大小；此限制适用于[引入项目并为其建立索引](/graph/api/externalconnectors-externalconnection-put-items?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0)时的请求正文。 |
| **N/A** | 属性的最大大小。 |

## <a name="throttling"></a>限制

当超过 [限制](throttling.md) 阈值时，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），并且请求失败。在失败请求的响应标头中会返回建议的等待时间。

限制行为可能取决于请求的类型和数量。例如，如果具有大量请求，则会限制所有请求类型。阈值限制因请求类型而异。因此，你可能会遇到写入受到限制，但仍允许读取的情况。
