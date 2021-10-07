---
title: externalConnection 资源类型
description: 连接是 Microsoft 服务中外部内容的逻辑Graph
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f7eeddc207206e6bcfcd526e8ac3e2cd00d481b3
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214733"
---
# <a name="externalconnection-resource-type"></a>externalConnection 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个逻辑容器，用于将外部源中的内容添加到 Microsoft Graph。

## <a name="methods"></a>方法

| 方法                                                           | 返回类型                                   | 说明 |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [创建 externalConnection](../api/externalconnectors-external-post-connections.md) | externalConnection                            | 通过发布到 connections 集合创建新的 externalConnection。 |
| [列出 externalConnections](../api/externalconnectors-externalconnection-list.md)    | externalConnection 集合                 | 获取 externalConnection 对象集合。 |
| [获取 externalConnection](../api/externalconnectors-externalconnection-get.md)       | externalConnection                            | 读取 externalConnection 对象的属性和关系。 |
| [更新 externalConnection](../api/externalconnectors-externalconnection-update.md) | externalConnection                            | 更新 externalConnection 对象。 |
| [删除 externalConnection](../api/externalconnectors-externalconnection-delete.md) | 无                                          | 删除 externalConnection 对象。 |
| [创建架构](../api/externalconnectors-externalconnection-post-schema.md)        | 无 *或*[架构](externalconnectors-schema.md)                 | 注册连接架构。 |
| [获取操作](../api/externalconnectors-connectionoperation-get.md)               | [connectionOperation](externalconnectors-connectionoperation.md) | 获取用于创建连接架构的异步请求的状态。 |
| [创建 externalItem](../api/externalconnectors-externalconnection-put-items.md)    | [externalItem](externalconnectors-externalitem.md)               | 通过发布到项目集合创建新的 externalItem。 |

## <a name="properties"></a>属性

| 属性      | 类型                              | 说明 |
|:--------------|:----------------------------------|:------------|
| configuration | [microsoft.graph.externalConnectors.configuration](externalconnectors-configuration.md) | 指定允许管理连接和索引连接内容的其他应用程序 ID。 可选。 |
| connectorId   |String                             | 应用Teams ID。 可选。|
| 说明   | String                            | 网站中显示的连接Microsoft 365 管理中心。 可选。 |
| id            | String                            | 开发人员为租户内的连接提供的唯Azure Active Directory ID。 长度必须在 3 到 32 个字符之间。 只能包含字母数字字符。 不能以 `Microsoft` 或 作为下列值之一：、 `None` `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` `TaskFabric` `PowerBI` `Assistant` `TopicEngine` `MSFT_All_Connectors` 。 必需。 |
| name          | 字符串                            | 要显示名称中显示的连接的Microsoft 365 管理中心。 最大长度为 128 个字符。 必需。 |
| searchSettings|[microsoft.graph.externalConnectors.searchSettings](../resources/externalconnectors-searchsettings.md)|配置此连接中内容的搜索体验的设置，例如搜索结果的显示模板。|
| state         | microsoft.graph.externalConnectors.connectionState                   | 指示连接的当前状态。 可能的值为 `draft` `ready` 、、 `obsolete` 和 `limitExceeded` 。 必填。 |

## <a name="relationships"></a>关系

| 关系 | 类型                                                     | 说明 |
|:-------------|:---------------------------------------------------------|:---|
| items        | [microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md) 集合               | 只读。可为空。 |
| operations   | [microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md) 集合 | 只读。可为空。 |
| schema       | [microsoft.graph.externalConnectors.schema](externalconnectors-schema.md)                                      | 只读。可为空。 |
| groups       | [microsoft.graph.externalConnectors.externalGroup](externalconnectors-externalgroup.md) 集合             | 只读。可为空。 |

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
