---
title: attributeSet 资源类型
description: 一个代表一组相关自定义安全属性定义的对象。
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 958ecbd900a98cfe9f91bf5d7fe526b2f4050bfa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077142"
---
# <a name="attributeset-resource-type"></a>attributeSet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个代表一组相关自定义安全属性定义的对象。

租户中可定义最多 500 `attributeSet` 个对象。 无法重命名或删除。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[List attributeSets](../api/directory-list-attributesets.md)|[attributeSet](../resources/attributeset.md) 集合|获取 [attributeSet 对象](../resources/attributeset.md) 及其属性的列表。|
|[获取 attributeSet](../api/attributeset-get.md)|[attributeSet](../resources/attributeset.md)|读取 [attributeSet](../resources/attributeset.md) 对象的属性和关系。|
|[创建 attributeSet](../api/directory-post-attributesets.md)|[attributeSet](../resources/attributeset.md)|创建新的 [attributeSet](../resources/attributeset.md) 对象。|
|[更新属性集](../api/attributeset-update.md)|[attributeSet](../resources/attributeset.md)|更新 [attributeSet 对象](../resources/attributeset.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|属性集的说明。 可最多为 128 个字符，并且包含 Unicode 字符。 稍后可更改。|
|id|String|租户中唯一的属性集的标识符。 可最多为 32 个字符，并且包含 Unicode 字符。 不能包含空格或特殊字符。 以后无法更改。 不区分大小写。|
|maxAttributesPerSet|Int32|可以在此属性集内定义的自定义安全属性的最大数量。 默认值为 `null`。 如果未指定，则管理员最多可以添加每个租户 500 个活动属性。 稍后可更改。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attributeSet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attributeSet",
  "description": "String",
  "id": "String (identifier)",
  "maxAttributesPerSet": "Integer"
}
```
