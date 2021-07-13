---
title: templateParameter 资源类型
description: 表示在管理模板中利用的参数。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4f533bc375e2d7e4a1e4ef2f7f801f248c1801c4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402395"
---
# <a name="templateparameter-resource-type"></a>templateParameter 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在管理模板中利用的参数。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|模板参数的说明。 可选。 只读。|
|displayName|String|template 显示名称参数的值。 必填。 只读。|
|jsonAllowedValues|String|模板参数的允许值，由 JSON 的序列化字符串表示。 可选。 只读。|
|jsonDefaultValue|String|模板参数的默认值，由 JSON 的序列化字符串表示。 必填。 只读。|
|valueType|managementParameterValueType|模板数据类型参数的值。 可取值为：`string`、`integer`、`boolean`、`guid`、`stringCollection`、`integerCollection`、`booleanCollection`、`guidCollection`、`unknownFutureValue`。 必填。 只读。|

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
