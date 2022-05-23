---
title: connectionQuota 资源类型
description: 表示包含有关外部连接配额利用率的计算信息的连接配额。
author: snlraju-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 68a8015115157bbc7ca12a9851c7386053e2d72a
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629213"
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
| itemsRemaining | Int64 | 最少两个值，一个表示 *连接中剩余的项* ，另一个 *表示租户级别的其他剩余项*。 <br/>以下公式表示用于计算最小数字的公式：<br/> 最小 (\{&#65279;连接\}_中的最大容量_ - \{_&#65279;连接_\}中的项数， \{_&#65279;租户配额_\} - \{_&#65279;在所有连接_\}) 索引的项目数。 <br/>如果连接未盈利，例如在预览连接器或预览内容体验中，则此属性只是连接中剩余项的数量。 |

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
