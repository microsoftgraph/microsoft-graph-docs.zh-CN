---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e6bbdb3287ca16020da7385dc3c268224590edd4
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60449395"
---
# <a name="auditresource-resource-type"></a>auditResource 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含审核资源的属性的类。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|显示名称。|
|ModifiedProperties|[auditProperty](../resources/intune-auditing-auditproperty.md) 集合|已修改属性列表。|
|type|String|审核资源的类型。|
|resourceId|String|审核资源的 ID。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



