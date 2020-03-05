---
title: onPremisesAgent 资源类型
description: onPremisesAgent 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff30f427c2aac754ba3cfda4082d590e95f5edd3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522240"
---
# <a name="onpremisesagent-resource-type"></a>onPremisesAgent 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示内部部署代理。 可将租户管理员安装的本地代理配置为访问/处理特定的[已发布资源](publishedresource.md)的请求。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 onPremisesAgents](../api/onpremisesagent-list.md) | [onPremisesAgent](onpremisesagent.md)集合 | 获取**onPremisesAgents**对象集合。 |
| [获取 onPremisesAgent](../api/onpremisesagent-get.md) | [onPremisesAgent](onpremisesagent.md) | 读取**onPremisesAgent**对象的属性和关系。 |
| [将 onPremisesAgent 分配给 onPremisesAgentGroup](../api/onpremisesagent-post-agentgroups.md) | 无 | 将**onPremisesAgent**分配给**onPremisesAgentGroup**。|
| [从 onPremisesAgentGroup 中删除 onpremisesAgent](../api/onpremisesagent-delete-agentgroups.md) | 无 | 从**onPremisesAgentGroup**中删除**onPremisesAgent** 。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|externalIp|String|由代理计算机的服务检测到的外部 IP 地址。 只读|
|id|String| OnPremisesAgent 的对象 id。 只读。|
|machineName|String|运行 aggent 的计算机的名称。 只读|
|状态|string| 可取值为：`active`、`inactive`。|
|publishingType|string| 可取值为：`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|agentGroups|[onPremisesAgentGroup](onpremisesagentgroup.md)集合| 向其分配**onPremisesAgent**的**onPremisesAgentGroups**的列表。 此为只读属性。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "baseType": "",
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
