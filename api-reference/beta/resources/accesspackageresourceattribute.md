---
title: accessPackageResourceAttribute 资源类型
description: 公开访问包请求者的属性的资源，以提供可用于为访问包做出审批决策的自定义信息。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9da68399fd09b6277499985fdc87512d7a5c5ae9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861336"
---
# <a name="accesspackageresourceattribute-resource-type"></a>accessPackageResourceAttribute 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

公开访问包请求者的属性的资源，以提供可用于为访问包做出审批决策的自定义信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|attributeDestination|[accessPackageResourceAttributeDestination](../resources/accesspackageresourceattributedestination.md)|有关如何设置属性的信息。|
|attributeName|String|最终系统中属性的名称。|
|attributeSource|[accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md)|有关在 **accessPackageAssignmentRequest** 实现时如何填充属性值的信息。|
|id|String|属性的唯一标识符。|
|isEditable|String| 指定请求者是否可以编辑现有属性值。|
|isPersistedOnAssignmentRemoval|布尔| 指定属性在工作分配结束后是否仍保留在最终系统中。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttribute",
  "attributeDestination": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeDestination"
  },
  "attributeName": "String",
  "attributeSource": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeSource"
  },
  "id": "String (identifier)",
  "isEditable": "Boolean",
}
```
