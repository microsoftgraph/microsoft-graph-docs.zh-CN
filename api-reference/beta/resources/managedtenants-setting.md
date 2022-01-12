---
title: 设置资源类型
description: 表示在基线中使用的设置。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 53eaf2dd4c3e97e183083f1a6c0d127ffbaefafd
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861292"
---
# <a name="setting-resource-type"></a>设置资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在基线中使用的设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|设置显示名称值。 必需。 只读。|
|jsonValue|String|设置为 JSON 字符串序列化的设置的值。 必需。 只读。|
|overwriteAllowed|Boolean|指示应用此设置时是否可以替代现有配置的标志。 必需。 只读。|
|valueType|managementParameterValueType|设置数据类型值。 可取值为：`string`、`integer`、`boolean`、`guid`、`stringCollection`、`integerCollection`、`booleanCollection`、`guidCollection`、`unknownFutureValue`。 必需。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.setting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.setting",
  "displayName": "String",
  "overwriteAllowed": "Boolean",
  "valueType": "String",
  "jsonValue": "String"
}
```
