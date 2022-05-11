---
title: externalConnection 资源类型
description: 连接是 Microsoft Graph 中外部内容的逻辑容器
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 417af041fc70ce86e921568b60059948754b942f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315697"
---
# <a name="externalconnection-resource-type"></a>externalConnection 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个逻辑容器，用于将外部源中的内容添加到 Microsoft Graph。

## <a name="methods"></a>方法

| 方法                                                           | 返回类型                                   | 说明 |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [创建 externalConnection](../api/externalconnectors-external-post-connections.md) | externalConnection                            | 通过发布到连接集合来创建新的 **externalConnection** 。 |
| [列出 externalConnections](../api/externalconnectors-externalconnection-list.md)    | externalConnection 集合                 | 获取 **externalConnection** 对象集合。 |
| [获取 externalConnection](../api/externalconnectors-externalconnection-get.md)       | externalConnection                            | 读取 **externalConnection** 对象的属性和关系。 |
| [更新 externalConnection](../api/externalconnectors-externalconnection-update.md) | externalConnection                            | 更新 **externalConnection** 对象。 |
| [删除 externalConnection](../api/externalconnectors-externalconnection-delete.md) | 无                                          | 删除 **externalConnection** 对象。 |
| [创建架构](../api/externalconnectors-externalconnection-post-schema.md)        | 无 *或*[架构](externalconnectors-schema.md)                 | 注册连接架构。 |
| [获取操作](../api/externalconnectors-connectionoperation-get.md)               | [connectionOperation](externalconnectors-connectionoperation.md) | 获取用于创建连接架构的异步请求的状态。 |
| [创建 externalItem](../api/externalconnectors-externalconnection-put-items.md)    | [externalItem](externalconnectors-externalitem.md)               | 通过发布到项目集合来创建新的 externalItem。 |
|[获取 connectionQuota](../api/externalconnectors-connectionquota-get.md)|[connectionQuota](../resources/externalconnectors-connectionquota.md)| 检索 **connectionQuota** 的属性和关系。 |

## <a name="properties"></a>属性

| 属性      | 类型                              | 说明 |
|:--------------|:----------------------------------|:------------|
| configuration | [microsoft.graph.externalConnectors.configuration](externalconnectors-configuration.md) | 指定允许管理连接和为连接中的内容编制索引的其他应用程序 ID。 可选。 |
| connectorId   |String                             | Teams应用 ID。 可选。|
| 说明   | String                            | Microsoft 365 管理中心中显示的连接的说明。 可选。 |
| id            | String                            | 开发人员提供的连接在Azure Active Directory租户中的唯一 ID。 长度必须介于 3 到 32 个字符之间。 必须仅包含字母数字字符。 不能以`Microsoft`以下值之一开头或为以下值之一：`None`、、`Exchange``Directory`、`ExchangeArchive`、`LinkedIn`、`OneDriveBusiness``Mailbox`、`SharePoint`、`Teams``Yammer`、、`Connectors`、`TaskFabric`、`PowerBI`、、`Assistant`、、、 `MSFT_All_Connectors``TopicEngine` 必填。 |
| ingestedItemsCount           | Int64                            |  引入到连接中的项数。 此值每 15 分钟刷新一次。 如果连接状态为 `draft`，则 **ingestedItemsCount** 将为 `null`. |
| name          | String                            | 要在Microsoft 365 管理中心中显示的连接的显示名称。 最大长度为 128 个字符。 必填。 |
| searchSettings|[microsoft.graph.externalConnectors.searchSettings](../resources/externalconnectors-searchsettings.md)|配置此连接中内容的搜索体验的设置，例如搜索结果的显示模板。|
| state         | microsoft.graph.externalConnectors.connectionState                   | 指示连接的当前状态。 可能的值是`draft`， `ready`和 `obsolete``limitExceeded`. 必填。 |

## <a name="relationships"></a>关系

| 关系 | 类型                                                     | 说明 |
|:-------------|:---------------------------------------------------------|:---|
| groups       | [microsoft.graph.externalConnectors.externalGroup](externalconnectors-externalgroup.md) 集合             | 只读。可为 Null。 |
| items        | [microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md) 集合               | 只读。可为空。 |
| operations   | [microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md) 集合 | 只读。可为 Null。 |
| 配额        | [microsoft.graph.externalConnectors.connectionQuota](externalconnectors-connectionquota.md)             | 只读。可为 Null。 |
| 模式       | [microsoft.graph.externalConnectors.schema](externalconnectors-schema.md)                                      | 只读。可为空。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "ingestedItemsCount": "Int64",
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
