---
title: onPremisesAgentGroup 资源类型
description: onPremisesAgentGroup 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 203d914098d6b7cb0b03715accac4958bcf53870
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522233"
---
# <a name="onpremisesagentgroup-resource-type"></a>onPremisesAgentGroup 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示本地代理组。 通过代理组，租户管理员可以分配特定的[代理](onpremisesagent.md)来服务特定[的已发布内部部署资源](publishedresource.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 onPremisesAgentGroups](../api/onpremisesagentgroup-list.md) | onPremisesAgentGroups 集合 | 获取**onPremisesAgentGroup**对象集合。 |
| [获取 onPremisesAgentGroup](../api/onpremisesagentgroup-get.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | 读取**onPremisesAgentGroup**对象的属性和关系。 |
| [创建 onPremisesAgentGroup](../api/onpremisesagentgroup-post.md)  | [onPremisesAgentGroup](onpremisesagentgroup.md) | 创建新的**onPremisesAgentGroup**。 |
| [更新 onPremisesAgentGroup](../api/onpremisesagentgroup-update.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | 更新**onPremisesAgentGroup**对象。 |
| [删除 onPremisesAgentGroup](../api/onpremisesagentgroup-delete.md) | 无 | 删除**onPremisesAgentGroup**对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|String|**OnPremisesAgentGroup**的显示名称。|
|id|String| **OnPremisesAgentGroup**的对象 ID。 只读。|
|isDefault|Boolean|指示**onPremisesAgentGroup**是否为默认代理组。 只有一个代理组可以是默认的**onPremisesAgentGroup** ，并由系统进行设置。|
|publishingType|string| 可取值为：`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|agent|[onPremisesAgent](onpremisesagent.md)集合| 分配给**onPremisesAgentGroup**的**onPremisesAgent**的列表。 只读。 可为 NULL。|
|publishedResources|[publishedResource](publishedresource.md)集合| 分配给**onPremisesAgentGroup**的**publishedResource**的列表。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "baseType": "",
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
