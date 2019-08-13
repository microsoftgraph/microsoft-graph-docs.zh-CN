---
title: rolePermission 资源类型
description: 包含为每个角色确定允许和不允许的权限的一组 ResourceActions。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c612e4c6201a3016b866eddc7e5e52d0b3238306
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369211"
---
# <a name="rolepermission-resource-type"></a>rolePermission 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含为每个角色确定允许和不允许的权限的一组 ResourceActions。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actions|String collection|允许的操作-已弃用|
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



