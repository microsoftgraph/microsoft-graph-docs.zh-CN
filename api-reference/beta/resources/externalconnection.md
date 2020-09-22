---
title: externalConnection 资源类型
description: 连接是 Microsoft Graph 中外部内容的逻辑容器
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 82a68c8670a1381263d0b6fd3704f9d6d900d1f0
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193139"
---
# <a name="externalconnection-resource-type"></a>externalConnection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将外部源中的内容添加到 Microsoft Graph 中的逻辑容器。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法

| 方法                                                           | 返回类型                                   | 说明 |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [创建 externalConnection](../api/external-post-connections.md) | externalConnection                            | 通过发布到 connections 集合创建新的 externalConnection。 |
| [列出 externalConnections](../api/externalconnection-list.md)    | externalConnection 集合                 | 获取 externalConnection 对象集合。 |
| [获取 externalConnection](../api/externalconnection-get.md)       | externalConnection                            | 读取 externalConnection 对象的属性和关系。 |
| [更新 externalConnection](../api/externalconnection-update.md) | externalConnection                            | 更新 externalConnection 对象。 |
| [删除 externalConnection](../api/externalconnection-delete.md) | 无                                          | 删除 externalConnection 对象。 |
| [创建架构](../api/externalconnection-post-schema.md)        | 无*或*[架构](schema.md)                 | 注册连接架构。 |
| [Get 操作](../api/connectionoperation-get.md)               | [connectionOperation](connectionoperation.md) | 获取用于创建连接架构的异步请求的状态。 |
| [创建 externalItem](../api/externalconnection-put-items.md)    | [externalItem](externalitem.md)               | 通过发布到 items 集合创建新的 externalItem。 |

## <a name="properties"></a>属性

| 属性      | 类型                              | 描述 |
|:--------------|:----------------------------------|:------------|
| configuration | [configuration](configuration.md) | 指定允许管理连接和索引连接中的内容的其他应用程序 Id。 可选。 |
| 说明   | 字符串                            | Microsoft 365 管理中心显示的连接的说明。 可选。 |
| id            | 字符串                            | 在 Azure Active Directory 租户中，开发人员提供的连接的唯一 ID。 最大长度为32个字符。 必须仅包含字母数字字符。 不能以 `Microsoft` 下列值开头，也不能为下列值之一：、、、、、、、、、、 `None` `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` 。 必需。 |
| name          | 字符串                            | 要显示在 Microsoft 365 管理中心中的连接的显示名称。 最大长度为128个字符。 必需。 |
| state         | connectionState                   | 指示连接的当前状态。 可能的值为 `draft` 、、 `ready` `obsolete` 和 `limitExceeded` 。 必填。 |

## <a name="relationships"></a>关系

| 关系 | 类型                                                     | 说明 |
|:-------------|:---------------------------------------------------------|:---|
| items        | [externalItem](externalitem.md) 集合               | 只读。可为空。 |
| operations   | [connectionOperation](connectionoperation.md) 集合 | 只读。 可为 Null。 |
| 架构       | [schema](schema.md)                                      | 只读。可为空。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "baseType": "",
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
