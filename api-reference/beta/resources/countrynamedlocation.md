---
title: countryNamedLocation 资源类型
description: 表示Azure Active Directory地区定义的命名位置。 命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。
ms.localizationpriority: medium
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d892b56d530ce80b9b34c5d0a3edfa0cae5d151a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336016"
---
# <a name="countrynamedlocation-resource-type"></a>countryNamedLocation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|countriesAndRegions|String 集合|ISO 3166-2 指定的两字母格式的国家/地区列表。|
|countryLookupMethod|countryLookupMethodType|确定用于确定用户所在的国家/地区的方法。 可能的值为 (`clientIpAddress` 和) 默认值 `authenticatorAppGps`。|
|createdDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 继承自 [namedLocation](../resources/namedLocation.md)。|
|displayName|String|位置的可读名称。 必需项。 继承自 [namedLocation](../resources/namedLocation.md)。|
|id|String|namedLocation 对象的标识符。 只读。 继承自 [namedLocation](../resources/namedLocation.md)。|
|includeUnknownCountriesAndRegions|Boolean|`true` 如果未映射到国家/地区或地区的 IP 地址应包含在命名位置中。 可选。 默认值为 `false`。|
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
  "countryLookupMethod": "countryLookedupMethodType",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "includeUnknownCountriesAndRegions": true,
  "modifiedDateTime": "String (timestamp)"
}
```

## <a name="see-also"></a>另请参阅

+ [什么是条件访问？](/azure/active-directory/conditional-access/overview)
+ [在条件访问策略中使用位置条件](/azure/active-directory/conditional-access/location-condition)


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "countryNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


