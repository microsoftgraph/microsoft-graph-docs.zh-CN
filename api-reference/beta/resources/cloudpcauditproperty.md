---
title: cloudPcAuditProperty 资源类型
description: 表示审核属性。这将显示已编辑的属性名称、旧值和新值。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 1f73733f0ace4526d3cbae226c963887d5af37ce
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211290"
---
# <a name="cloudpcauditproperty-resource-type"></a>cloudPcAuditProperty 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示审核属性。这将显示已编辑的属性名称、旧值和新值。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

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
