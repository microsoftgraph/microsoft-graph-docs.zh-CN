---
title: rolePermission 资源类型
description: 包含一组 ResourceActions，用于确定每个角色的允许和不允许的权限。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 288b2668e0156644f1c12ad8b87dfeba9e41e9a7
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736711"
---
# <a name="rolepermission-resource-type"></a>rolePermission 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含一组 ResourceActions，用于确定每个角色的允许和不允许的权限。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|resourceActions|[resourceAction](../resources/intune-rbac-resourceaction.md) 集合|每个资源操作都包含一组允许和不允许的权限。|

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





