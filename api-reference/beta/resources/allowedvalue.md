---
title: allowedValue 资源类型
description: 自定义安全属性定义允许的预定义值。
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 21e6b1836ae23e1cc6b7c78053ff458ac934087e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077504"
---
# <a name="allowedvalue-resource-type"></a>allowedValue 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

自定义安全属性定义允许的预定义值。

每个 `allowedValue` [customSecurityAttributeDefinition](customsecurityattributedefinition.md)可定义最多 100 个对象。 无法重命名或删除此对象，但可以使用 [Update allowedValue](../api/../api/allowedvalue-update.md) 操作停用该对象。 此对象定义为 [customSecurityAttributeDefinition](customsecurityattributedefinition.md) 资源的导航属性，并且仅在 上返回其值 `$expand` 。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 allowedValues](../api/customsecurityattributedefinition-list-allowedvalues.md)|[allowedValue](../resources/allowedvalue.md) 集合|获取 [allowedValue 对象](../resources/allowedvalue.md) 及其属性的列表。|
|[获取 allowedValue](../api/allowedvalue-get.md)|[allowedValue](../resources/allowedvalue.md)|读取 [allowedValue](../resources/allowedvalue.md) 对象的属性和关系。|
|[创建 allowedValue](../api/customsecurityattributedefinition-post-allowedvalues.md)|[allowedValue](../resources/allowedvalue.md)|创建新的 [allowedValue](../resources/allowedvalue.md) 对象。|
|[更新 allowedValue](../api/allowedvalue-update.md)|[allowedValue](../resources/allowedvalue.md)|更新 [allowedValue 对象](../resources/allowedvalue.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| id | String | 预定义值的标识符。 可最多为 64 个字符，并且包含 Unicode 字符。 可以包含空格，但不允许使用某些特殊字符。 以后无法更改。 区分大小写。 |
|isActive|布尔|指示预定义值是处于活动状态还是已停用。 如果设置为 `false` ，则此预定义值不能分配给任何其他受支持的目录对象。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.allowedValue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.allowedValue",
  "id": "String (identifier)",
  "isActive": "Boolean"
}
```
