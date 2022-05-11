---
title: connectionQuota 资源类型
description: 表示包含有关外部连接配额利用率的计算信息的连接配额。
author: josmoran
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 968d0154a1a0bbc5fe33bdcad1123c0944e854fb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316540"
---
# <a name="connectionquota-resource-type"></a>connectionQuota 资源类型

命名空间：microsoft.graph.externalConnectors

表示包含有关外部连接配额利用率的计算信息的 [连接](externalconnectors-externalconnection.md) 配额。 它通过考虑针对 Microsoft Graph 连接器的租户级配额引入连接的项目，返回可引入到连接中的允许项数。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
| [获取 connectionQuota](../api/externalconnectors-connectionquota-get.md) |[connectionQuota](../resources/externalconnectors-connectionquota.md)| 检索 **connectionQuota** 的属性和关系。 |

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| itemsRemaining | Int64 | 返回包含以下数据的范围内的最小数字： *连接中剩余的项* 和 *租户级别的剩余项*。 以下公式表示用于计算最小数字的公式： `min(max capacity in the connection – number of items in the connection, tenant quota – number of items indexed in all connections)`。 如果连接 (预览连接器或预览内容体验) 非规范化，则返回连接中的剩余项数。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.connectionQuota",
  "openType": false
}
-->

``` json
{
  "itemsRemaining": "Int64"
}
```
