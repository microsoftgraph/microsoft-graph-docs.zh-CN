---
title: externalConnection 资源类型
description: 从外部源到 Microsoft 搜索的连接。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 78752e2fe3375c10dcce57e3ba23e890b0ab66b5
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704176"
---
# <a name="externalconnection-resource-type"></a>externalConnection 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从外部源到 Microsoft 搜索的连接。

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

| 属性      | 类型                              | 说明 |
|:--------------|:----------------------------------|:------------|
| 设置 | [configuration](configuration.md) | 指定允许管理连接和索引连接中的内容的其他应用程序 Id。 可选。 |
| 说明   | String                            | Microsoft 365 管理中心显示的连接的说明。 可选。 |
| id            | String                            | 在 Azure Active Directory 租户中，开发人员提供的连接的唯一 ID。 最大长度为32个字符。 必须仅包含字母数字字符。 不能以`Microsoft`下列值开头，也不能为`None`下列`Directory`值`Exchange`之一`ExchangeArchive`： `LinkedIn`、 `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer`、、、、、、 `Connectors`、、、。 必需。 |
| name          | String                            | 要显示在 Microsoft 365 管理中心中的连接的显示名称。 最大长度为128个字符。 必需。 |

## <a name="relationships"></a>关系

| 关系 | 类型                                                     | 说明 |
|:-------------|:---------------------------------------------------------|:---|
| items        | [externalItem](externalitem.md)集合               | 只读。可为空。 |
| operations   | [connectionOperation](connectionoperation.md)集合 | 只读。 可为 Null。 |
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
  "name": "String"
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
