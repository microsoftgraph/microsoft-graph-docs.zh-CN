---
title: cloudPcAuditProperty 资源类型
description: 表示审核属性。这将显示已编辑的属性名称、旧值和新值。
author: ecmadao
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 769ba5aa685755477a0ee0dbcdaa05696ed96a79
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767200"
---
# <a name="cloudpcauditproperty-resource-type"></a>cloudPcAuditProperty 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示审核属性。这将显示已编辑的属性名称、旧值和新值。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|显示名称。|
|oldValue|String|旧值。|
|NewValue|String|新值。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditProperty"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```
