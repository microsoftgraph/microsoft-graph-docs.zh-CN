---
title: onPremisesAgentGroup 资源类型
description: onPremisesAgentGroup 资源类型。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 5751e01ab6e7645416a8a8fde5c30f09c38a3d22
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956916"
---
# <a name="onpremisesagentgroup-resource-type"></a>onPremisesAgentGroup 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示本地代理组。 通过代理组，租户管理员能够分配特定 [代理](onpremisesagent.md) ，为 [发布的特定本地资源提供服务](publishedresource.md)。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 onPremisesAgentGroups](../api/onpremisesagentgroup-list.md) | onPremisesAgentGroups 集合 | 获取 **onPremisesAgentGroup** 对象集合。 |
| [获取 onPremisesAgentGroup](../api/onpremisesagentgroup-get.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | 读取 **onPremisesAgentGroup** 对象的属性和关系。 |
| [创建 onPremisesAgentGroup](../api/onpremisesagentgroup-post.md)  | [onPremisesAgentGroup](onpremisesagentgroup.md) | 创建新的 **onPremisesAgentGroup**。 |
| [更新 onPremisesAgentGroup](../api/onpremisesagentgroup-update.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | 更新 **onPremisesAgentGroup** 对象。 |
| [删除 onPremisesAgentGroup](../api/onpremisesagentgroup-delete.md) | 无 | 删除 **onPremisesAgentGroup** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|String|**onPremisesAgentGroup 的显示名称**。|
|id|String| **onPremisesAgentGroup 的对象** ID。 只读。|
|isDefault|Boolean|指示 **onPremisesAgentGroup** 是否为默认代理组。 只有一个代理组可以是默认的 **onPremisesAgentGroup，** 并且由系统设置。|
|publishingType|String| 可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|agents|[onPremisesAgent](onpremisesagent.md) 集合| 分配给 **onPremisesAgentGroup** 的 **onPremisesAgent 列表**。 只读。 可为 Null。|
|publishedResources|[publishedResource](publishedresource.md) 集合| 分配给 **onPremisesAgentGroup** 的 **publishedResource** 列表。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "publishingType": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgentGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



