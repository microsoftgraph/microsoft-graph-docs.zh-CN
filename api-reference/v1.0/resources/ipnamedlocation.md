---
title: ipNamedLocation 资源类型
description: 表示由 IP 范围定义的 Azure Active Directory 命名位置。 命名位置是定义网络位置的自定义规则，之后可在条件访问策略中使用。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5f76d5bb27a17ec0cc642479f3808dfbc8a45f66
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159393"
---
# <a name="ipnamedlocation-resource-type"></a>ipNamedLocation 资源类型

命名空间：microsoft.graph

表示由 IP 范围定义的 Azure Active Directory 命名位置。 命名位置是定义网络位置的自定义规则，之后可在条件访问策略中使用。

继承自 [namedLocation](../resources/namedLocation.md)

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 ipNamedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [ipNamedLocation](ipNamedLocation.md) 集合 | 获取组织 **的所有 ipNamedLocation** 对象。 |
| [创建 ipNamedLocation](../api/conditionalaccessroot-post-namedlocations.md) | [ipNamedLocation](ipNamedLocation.md) | 创建新的 **ipNamedLocation** 对象。 |
| [获取 ipNamedLocation](../api/ipnamedlocation-get.md) | [ipNamedLocation](ipnamedlocation.md) | 读取 **ipNamedLocation** 对象的属性和关系。 |
| [更新 ipNamedLocation](../api/ipnamedlocation-update.md) | [ipNamedLocation](ipnamedlocation.md) | 更新 **ipNamedLocation** 对象。 |
| [删除 ipNamedLocation](../api/ipnamedlocation-delete.md) | 无 | 删除 **ipNamedLocation** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。 继承自 [namedLocation](../resources/namedLocation.md)。|
|displayName|String|位置的可读名称。|
|id|String|namedLocation 对象的标识符。 只读。 继承自 [namedLocation](../resources/namedLocation.md)。|
|ipRanges|[ipRange](iprange.md) 集合|IPv4 CIDR 格式的 IP 地址范围列表 (例如 1.2.3.4/32) IETF RFC596 中任何允许的 IPv6 格式。|
|isTrusted|布尔值|如果明确信任此位置，则其为 True。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的位置的上次修改日期和时间，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。 继承自 [namedLocation](../resources/namedLocation.md)。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipNamedLocation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "ipRanges": [{"@odata.type": "microsoft.graph.ipRange"}],
  "isTrusted": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ipNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

