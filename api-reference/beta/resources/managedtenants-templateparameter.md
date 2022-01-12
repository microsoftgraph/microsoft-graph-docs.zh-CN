---
title: templateParameter 资源类型
description: 表示在管理模板中利用的参数。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a2fe8cc543f60e2e862af65b9e47f6a84389e453
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791867"
---
# <a name="templateparameter-resource-type"></a>templateParameter 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在管理模板中利用的参数。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|模板参数的说明。 可选。 只读。|
|displayName|String|template 显示名称参数的值。 必需。 只读。|
|jsonAllowedValues|String|模板参数的允许值由 JSON 的序列化字符串表示。 可选。 只读。|
|jsonDefaultValue|String|模板参数的默认值，由 JSON 的序列化字符串表示。 必需。 只读。|
|valueType|managementParameterValueType|模板数据类型的值。 可取值为：`string`、`integer`、`boolean`、`guid`、`stringCollection`、`integerCollection`、`booleanCollection`、`guidCollection`、`unknownFutureValue`。 必需。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.templateParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.templateParameter",
  "displayName": "String",
  "description": "String",
  "valueType": "String",
  "jsonDefaultValue": "String",
  "jsonAllowedValues": "String"
}
```
