---
title: Microsoft Graph 连接器 API 限制
description: Microsoft Graph 连接器 API 限制
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 6ab757d16a10f2291ad9bac5034e9fe7357a7188
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645734"
---
# <a name="microsoft-graph-connector-api-limits"></a>Microsoft Graph 连接器 API 限制

本主题介绍 Microsoft Graph 连接器的实施和运行限制。 设计连接器时，请牢记这些限制。

## <a name="connection-limits"></a>连接限制

| **限制** | **说明** |
| --- | --- |
| **10 个连接** | 每个 Microsoft 365 租户的最大[连接](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true)资源数。 |
| **700,000 项** | 每个连接的最大[项目](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)数。 |
| **70 GB** | 连接的最大字节大小。 |

## <a name="schema-limits"></a>架构限制

| **限制** | **说明** |
| --- | --- |
| **128 个属性** | 可以在[架构](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true)中定义的最大数量的属性，描述通过连接引入的数据。 |

## <a name="group-limits"></a>组限制

| **限制** | **说明** |
| --- | --- |
| 100,000 | 每个 Microsoft 365 租户的最大[外部组](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true)数量。 |
| **1000 个请求/秒** | 组管理[限制](#throttling)阈值中每秒允许的最大请求数。 |

## <a name="item-ingestion"></a>项引入

| **限制** | **说明** |
| --- | --- |
| **每秒 4 个项目（每小时 250 MB）** | 通过连接引入项目的吞吐量限制。 |
| **4 MB** | 项目的最大大小；此限制适用于[引入项目并为其建立索引](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true)时的请求正文。 |
| **N/A** | 属性的最大大小。 |

## <a name="throttling"></a>限制

超出[限制](throttling.md)阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步请求。限制发生时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在此场景中，写入受限，但仍允许读取。
