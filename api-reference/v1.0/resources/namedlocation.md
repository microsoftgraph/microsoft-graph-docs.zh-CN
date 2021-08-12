---
title: namedLocation 资源类型
description: 这是表示命名位置的Azure Active Directory类。 命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5083e526fcf1d9c4a6b844faa4584f7193144f0a813a53fa3e8446411e6d47f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152360"
---
# <a name="namedlocation-resource-type"></a>namedLocation 资源类型

命名空间：microsoft.graph

这是表示命名位置的Azure Active Directory类。 命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 namedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [namedLocation](namedLocation.md) 集合 | 获取 **组织的所有 namedLocation** 对象。 |
| [获取 namedLocation](../api/namedlocation-get.md) | [namedLocation](namedlocation.md) | 读取 **namedLocation** 对象的属性和关系。 |
| [删除 namedLocation](../api/namedlocation-delete.md) | 无 | 删除 **namedLocation** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|displayName|String|位置的可读名称。|
|id|String|namedLocation 对象的标识符。 只读。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的位置的上次修改日期和时间，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "namedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

