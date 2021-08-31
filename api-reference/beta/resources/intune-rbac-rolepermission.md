---
title: rolePermission 资源类型
description: 包含一组 ResourceActions，用于确定每个角色的允许和不允许的权限。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 23e0105ee67fdf26d0edf97a3074281150b98745
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58757865"
---
# <a name="rolepermission-resource-type"></a>rolePermission 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含一组 ResourceActions，用于确定每个角色的允许和不允许的权限。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actions|String collection|允许的操作 - 已弃用|
|resourceActions|[resourceAction](../resources/intune-rbac-resourceaction.md) 集合|资源操作每个包含一组允许和不允许的权限。|

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



