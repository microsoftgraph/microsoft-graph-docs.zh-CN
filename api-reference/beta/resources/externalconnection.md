---
title: externalConnection 资源类型
description: 连接是 Microsoft Graph 中外部内容的逻辑容器
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4355ffe51fe1b160c7fb486272e85f2b2cf0bf2c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161699"
---
# <a name="externalconnection-resource-type"></a>externalConnection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将外部源中的内容添加到 Microsoft Graph 的逻辑容器。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法

| 方法                                                           | 返回类型                                   | 说明 |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [创建 externalConnection](../api/external-post-connections.md) | externalConnection                            | 通过发布到 connections 集合创建新的 externalConnection。 |
| [列出 externalConnections](../api/externalconnection-list.md)    | externalConnection 集合                 | 获取 externalConnection 对象集合。 |
| [获取 externalConnection](../api/externalconnection-get.md)       | externalConnection                            | 读取 externalConnection 对象的属性和关系。 |
| [更新 externalConnection](../api/externalconnection-update.md) | externalConnection                            | 更新 externalConnection 对象。 |
| [删除 externalConnection](../api/externalconnection-delete.md) | 无                                          | 删除 externalConnection 对象。 |
| [创建架构](../api/externalconnection-post-schema.md)        | 无 *或*[架构](schema.md)                 | 注册连接架构。 |
| [获取操作](../api/connectionoperation-get.md)               | [connectionOperation](connectionoperation.md) | 获取异步请求的状态以创建连接架构。 |
| [创建 externalItem](../api/externalconnection-put-items.md)    | [externalItem](externalitem.md)               | 通过发布到项目集合创建新的 externalItem。 |

## <a name="properties"></a>属性

| 属性      | 类型                              | 说明 |
|:--------------|:----------------------------------|:------------|
| configuration | [configuration](configuration.md) | 指定允许管理连接和索引连接内容的其他应用程序 ID。 可选。 |
| 说明   | String                            | Microsoft 365 管理中心中显示的连接说明。 可选。 |
| id            | String                            | 开发人员提供的 Azure Active Directory 租户内连接的唯一 ID。 最大长度为 32 个字符。 必须仅包含字母数字字符。 不能以下列值开头或为下列值之一 `Microsoft` ： ， ， ， ， `None` `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` 。 `Connectors` 必需。 |
| 名称          | String                            | 要显示名称 Microsoft 365 管理中心中显示的连接的列表。 最大长度为 128 个字符。 必需。 |
| state         | connectionState                   | 指示连接的当前状态。 可能的值是 `draft` ， `ready` 和 `obsolete` `limitExceeded` 。 必填。 |

## <a name="relationships"></a>关系

| 关系 | 类型                                                     | 说明 |
|:-------------|:---------------------------------------------------------|:---|
| items        | [externalItem](externalitem.md) 集合               | 只读。可为空。 |
| operations   | [connectionOperation](connectionoperation.md) 集合 | 只读。 可为 NULL。 |
| 架构       | [schema](schema.md)                                      | 只读。可为空。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "keyProperty": "id"
}-->

```json
{
  "configuration": {"@odata.type": "microsoft.graph.configuration"},
  "description": "String",
  "id": "String (identifier)",
  "name": "String",
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
