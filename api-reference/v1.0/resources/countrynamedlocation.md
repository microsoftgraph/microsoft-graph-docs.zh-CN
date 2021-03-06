---
title: countryNamedLocation 资源类型
description: 表示Azure Active Directory地区定义的命名位置。 命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 531942e5026e2fc3d4d9ed3311d9130275d5a853
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443163"
---
# <a name="countrynamedlocation-resource-type"></a>countryNamedLocation 资源类型

命名空间：microsoft.graph

表示Azure Active Directory地区定义的命名位置。 命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。

继承自 [namedLocation](../resources/namedLocation.md)

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 countryNamedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [countryNamedLocation](countryNamedLocation.md) 集合 | 获取 **组织的所有 countryNamedLocation** 对象。 |
| [创建 countryNamedLocation](../api/conditionalaccessroot-post-namedlocations.md) | [countryNamedLocation](countryNamedLocation.md) | 创建新的 **countryNamedLocation** 对象。 |
| [获取 countryNamedLocation](../api/countrynamedlocation-get.md) | [countryNamedLocation](countrynamedlocation.md) | 读取 **countryNamedLocation** 对象的属性和关系。 |
| [更新 countryNamedLocation](../api/countrynamedlocation-update.md) | [countryNamedLocation](countrynamedlocation.md) | 更新 **countryNamedLocation** 对象。 |
| [删除 countryNamedLocation](../api/countrynamedlocation-delete.md) | 无 | 删除 **countryNamedLocation** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|countriesAndRegions|字符串集合|ISO 3166-2 指定的两字母格式的国家/地区列表。|
|countryLookupMethod|countryLookupMethodType|确定用于确定用户所在的国家/地区的方法。 可能的值为 `clientIpAddress` 和 `authenticatorAppGps`。|
|createdDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 继承自 [namedLocation](../resources/namedLocation.md)。|
|displayName|String|位置的可读名称。 继承自 [namedLocation](../resources/namedLocation.md)。|
|id|String|namedLocation 对象的标识符。 只读。 继承自 [namedLocation](../resources/namedLocation.md)。|
|includeUnknownCountriesAndRegions|布尔|如此 如果未映射到国家/地区或地区的 IP 地址应包含在命名的位置。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的位置的上次修改日期和时间，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 继承自 [namedLocation](../resources/namedLocation.md)。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation"
}-->

```json
{
  "countriesAndRegions": ["String"],
  "countryLookupMethod": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "includeUnknownCountriesAndRegions": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "countryNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
