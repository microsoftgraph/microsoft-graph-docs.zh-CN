---
title: 连接器资源类型
description: 表示应用程序代理连接器。
author: japere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3e42bc42c1989e530f7b7f307da3963407ded112
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027165"
---
# <a name="connector-resource-type"></a>连接器资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

连接器是位于本地的轻型代理，便于与 [AZURE AD 应用程序代理](https://aka.ms/whyappproxy) 服务的出站连接。 每个连接器都是 [connectorGroup](connectorgroup.md)的一部分。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [List connectors](../api/connector-list.md) | [连接器](connector.md) 集合 | 检索连接器对象的列表。 | 
| [Get connector](../api/connector-get.md) | [连接器](connector.md) | 读取连接器对象的属性和关系。 |
| [List memberOf](../api/connector-list-memberof.md) | [connectorGroup](connectorgroup.md) 集合 | 列出连接器所属的 connectorGroup 对象集合。 |
| [Add connector to connectorGroup](../api/connector-post-memberof.md)| [connectorGroup](connectorgroup.md) | 将连接器添加到 connectorGroup。 |


## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|externalIp|String| 连接器服务器检测到的外部 IP 地址。 只读。 |
|id|String| 连接器的唯一标识符。 只读。 |
|machineName|String| 连接器已安装并在其上运行的计算机名称。 |
|状态|string| 指示连接器的状态。 可能的值是：`active`、`inactive`。 只读。 |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|memberOf|[connectorGroup](connectorgroup.md) 集合| 连接器所属的 connectorGroup。 只读。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connector"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


