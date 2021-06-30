---
title: cloudPcAuditResource 资源类型
description: 表示审核资源。这将显示具有多个已编辑属性的目标已编辑资源实体。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ebd61a14680c5e5f2917e273456bcce60672149e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211287"
---
# <a name="cloudpcauditresource-resource-type"></a>cloudPcAuditResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示审核资源。这将显示具有多个已编辑属性的目标已编辑资源实体。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|资源实体显示名称。|
|ModifiedProperties|[cloudPcAuditProperty](../resources/cloudpcauditproperty.md) 集合|已修改属性的列表。|
|type|String|审核资源的类型。|
|resourceId|String|审核资源的 ID。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditResource"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```
