---
title: assignmentFilterSupportedProperty 资源类型
description: 表示有关该属性的信息，该属性在构建 AssignmentFilter 规则时受支持。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 339f220b9508487735e2473133e61c2682263c05
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074946"
---
# <a name="assignmentfiltersupportedproperty-resource-type"></a>assignmentFilterSupportedProperty 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示有关该属性的信息，该属性在构建 AssignmentFilter 规则时受支持。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|DataType|String|属性的数据类型。|
|isCollection|Boolean|指示属性是否是集合类型。|
|name|String|属性的名称。|
|propertyRegexConstraint|String|正则表达式字符串，用于对属性值进行验证。|
|supportedOperators|[assignmentFilterOperator](../resources/intune-policyset-assignmentfilteroperator.md) 集合|此属性上所有受支持的运算符的列表。|
|supportedValues|String collection|此名称的所有受支持值的列表，如果所有内容均受支持，则为空。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterSupportedProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterSupportedProperty",
  "dataType": "String",
  "isCollection": true,
  "name": "String",
  "propertyRegexConstraint": "String",
  "supportedOperators": [
    "String"
  ],
  "supportedValues": [
    "String"
  ]
}
```



