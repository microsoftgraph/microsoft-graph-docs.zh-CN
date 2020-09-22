---
title: rolePermission 资源类型
description: 包含为每个角色确定允许和不允许的权限的一组 ResourceActions。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d8627639d0eabed4392ed3d6763731dc4b65113c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039487"
---
# <a name="rolepermission-resource-type"></a>rolePermission 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含为每个角色确定允许和不允许的权限的一组 ResourceActions。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actions|String 集合|允许的操作-已弃用|
|resourceActions|[resourceAction](../resources/intune-rbac-resourceaction.md) 集合|每个包含一组允许和不允许的权限的资源操作。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```






