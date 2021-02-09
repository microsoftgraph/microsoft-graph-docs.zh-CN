---
title: onPremisesAgent 资源类型
description: onPremisesAgent 资源类型。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 59ee11bb952c85695b8c20daa1e040c8899740b9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158350"
---
# <a name="onpremisesagent-resource-type"></a>onPremisesAgent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示本地代理。 租户管理员安装本地代理可以配置为访问/处理对特定已发布 [资源的请求](publishedresource.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 onPremisesAgents](../api/onpremisesagent-list.md) | [onPremisesAgent](onpremisesagent.md) 集合 | 获取 **onPremisesAgents** 对象集合。 |
| [获取 onPremisesAgent](../api/onpremisesagent-get.md) | [onPremisesAgent](onpremisesagent.md) | 读取 **onPremisesAgent** 对象的属性和关系。 |
| [将 onPremisesAgent 分配给 onPremisesAgentGroup](../api/onpremisesagent-post-agentgroups.md) | 无 | 将 **onPremisesAgent** 分配给 **onPremisesAgentGroup**。|
| [从 onPremisesAgentGroup 中删除 onpremisesAgent](../api/onpremisesagent-delete-agentgroups.md) | 无 | 从 **onPremisesAgentGroup** 中删除 **onPremisesAgent**。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|externalIp|String|代理计算机的服务检测到的外部 IP 地址。 只读|
|id|String| onPremisesAgent 的对象 ID。 只读。|
|machineName|String|正在运行的计算机的名称。 只读|
|状态|string| 可取值为：`active`、`inactive`。|
|publishingType|string| 可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|agentGroups|[onPremisesAgentGroup](onpremisesagentgroup.md) 集合| **onPremisesAgent 分配到** 的 **onPremisesAgentGroups** 列表。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "keyProperty": "id"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string",
  "supportedPublishingTypes": ["string"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



