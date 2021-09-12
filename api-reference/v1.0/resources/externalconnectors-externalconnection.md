---
title: externalConnection 资源类型
description: 连接是 Microsoft 服务中外部内容的逻辑Graph
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1d47af18cc6869b53c6356df9b2bf0563a64655c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007220"
---
# <a name="externalconnection-resource-type"></a>externalConnection 资源类型

命名空间：microsoft.graph.externalConnectors

一个逻辑容器，用于将外部源中的内容添加到 Microsoft Graph。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[创建 externalConnection](../api/externalconnectors-external-post-connections.md)|[externalConnection](../resources/externalconnectors-externalconnection.md)|创建新的 [externalConnection](../resources/externalconnectors-externalconnection.md) 对象。|
|[列出 externalConnections](../api/externalconnectors-externalconnection-list.md)|[externalConnection](../resources/externalconnectors-externalconnection.md) 集合|获取 [externalConnection 对象](../resources/externalconnectors-externalconnection.md) 及其属性的列表。|
|[获取 externalConnection](../api/externalconnectors-externalconnection-get.md)|[externalConnection](../resources/externalconnectors-externalconnection.md)|读取 [externalConnection 对象的属性和](../resources/externalconnectors-externalconnection.md) 关系。|
|[更新 externalConnection](../api/externalconnectors-externalconnection-update.md)|[externalConnection](../resources/externalconnectors-externalconnection.md)|更新 [externalConnection 对象](../resources/externalconnectors-externalconnection.md) 的属性。|
|[删除 externalConnection](../api/externalconnectors-externalconnection-delete.md)|None|删除 [externalConnection](../resources/externalconnectors-externalconnection.md) 对象。|
|[创建架构](../api/externalconnectors-schema-create.md)|[schema](../resources/externalconnectors-schema.md)|创建新的架构对象。|
|[创建 externalItem](../api/externalconnectors-externalitem-create.md)|[externalItem](../resources/externalconnectors-externalitem.md)|创建新的 externalItem 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|configuration|[microsoft.graph.externalConnectors.configuration](../resources/externalconnectors-configuration.md)|指定允许管理连接和索引连接内容的其他应用程序 ID。 可选。|
|说明|String|网站中显示的连接Microsoft 365 管理中心。 可选。|
|id|String| 开发人员提供在租户内连接的唯Azure Active Directory ID。 长度必须在 3 到 32 个字符之间。 只能包含字母数字字符。 不能以 `Microsoft` 或 作为下列值之一：、 `None` `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` `TaskFabric` `PowerBI` `Assistant` `TopicEngine` `MSFT_All_Connectors` 。 必需。 |
|name|String|要显示名称中显示的连接的Microsoft 365 管理中心。 最大长度为 128 个字符。 必填。|
|state|microsoft.graph.externalConnectors.connectionState|指示连接的当前状态。 可取值为：`draft`、`ready`、`obsolete`、`limitExceeded`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|items|[microsoft.graph.externalConnectors.externalItem](../resources/externalconnectors-externalitem.md) 集合|只读。可为空。|
|operations|[microsoft.graph.externalConnectors.connectionOperation](../resources/externalconnectors-connectionoperation.md) 集合|只读。可为 Null。|
|schema|[microsoft.graph.externalConnectors.schema](../resources/externalconnectors-schema.md)|只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "state": "String"
}
```

