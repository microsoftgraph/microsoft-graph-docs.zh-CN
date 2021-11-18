---
title: customSecurityAttributeDefinition 资源类型
description: 一个代表自定义安全属性架构的对象 (键值对) 。
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 390af00d09d2b54fde5bf1cf510ad1752038d3fa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077680"
---
# <a name="customsecurityattributedefinition-resource-type"></a>customSecurityAttributeDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个代表自定义安全属性架构的对象 (键值对) 。 例如，自定义安全属性名称、说明、数据类型和允许的值。

租户中可定义最多 500 个活动对象。 无法重命名或删除该对象，但可以使用 `customSecurityAttributeDefiniton` [Update customSecurityAttributeDefinition](../api/customsecurityattributedefinition-update.md) 操作停用该对象。 必须是属性集的一部分。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 customSecurityAttributeDefinitions](../api/directory-list-customsecurityattributedefinitions.md)|[customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) 集合|获取 [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) 对象及其属性的列表。|
|[获取 customSecurityAttributeDefinition](../api/customsecurityattributedefinition-get.md)|[customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md)|读取 [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) 对象的属性和关系。|
|[创建 customSecurityAttributeDefinition](../api/directory-post-customsecurityattributedefinitions.md)|[customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md)|创建新的 [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) 对象。|
|[更新 customSecurityAttributeDefinition](../api/customsecurityattributedefinition-update.md)|[customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md)|更新 [customSecurityAttributeDefinition 对象](../resources/customsecurityattributedefinition.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|attributeSet|String|属性集的名称。 不区分大小写。|
|说明|String|自定义安全属性的说明。 可最多为 128 个字符，并且包含 Unicode 字符。 稍后可更改。|
|id|String|自定义安全属性的标识符，它是属性集名称和自定义安全属性名称的组合，由下划线字符 (`attributeSet` _ `name`) 。 `id`该属性是自动生成的，不能设置。 不区分大小写。|
|isCollection|布尔|指示是否可以将多个值分配给自定义安全属性。 以后无法更改。 如果 `type` 设置为 Boolean， `isCollection` 则不能设置为 true。|
|isSearchable|布尔|指示是否将为自定义安全属性值编制索引，以在分配了属性值的对象上搜索。 以后无法更改。|
|name|String|自定义安全属性的名称。 在属性集内必须是唯一的。 可最多为 32 个字符，并且包含 Unicode 字符。 不能包含空格或特殊字符。 以后无法更改。 不区分大小写。|
|status|String|指定自定义安全属性是处于活动状态还是已停用。 可接受的值为 和 `Available` `Deprecated` 。 稍后可更改。|
|type|String|自定义安全属性值的数据类型。 支持的类型包括 `Boolean` 、 `Integer` 和 `String` 。 以后无法更改。|
|usePreDefinedValuesOnly|布尔|指示是否只能将预定义值分配给自定义安全属性。 如果设置为 false，则允许自由格式的值。 稍后可以从 true 更改为 false，但无法从 false 更改为 true。 如果 `type` 设置为 Boolean， `usePreDefinedValuesOnly` 则不能设置为 true。 |


## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|allowedValues|[allowedValue](../resources/allowedvalue.md) 集合|为此自定义安全属性预定义的值。<br><br>默认情况下不会返回此导航属性，必须在查询中指定 `$expand` 该属性。 例如，`/directory/customSecurityAttributeDefinitions?$expand=allowedValues`。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSecurityAttributeDefinition",
  "attributeSet": "String",
  "description": "String",
  "id": "String (identifier)",
  "isCollection": "Boolean",
  "isSearchable": "Boolean",
  "name": "String",
  "status": "String",
  "type": "String",
  "usePreDefinedValuesOnly": "Boolean"
}
```
