---
title: roleScopeTag 资源类型
description: 角色范围标记
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4106ba2b3764621c94db52d92ca1d7b5e213dee0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039480"
---
# <a name="rolescopetag-resource-type"></a>roleScopeTag 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

角色范围标记

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 roleScopeTags](../api/intune-rbac-rolescopetag-list.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) 集合|列出 [roleScopeTag](../resources/intune-rbac-rolescopetag.md) 对象的属性和关系。|
|[获取 roleScopeTag](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|读取 [roleScopeTag](../resources/intune-rbac-rolescopetag.md) 对象的属性和关系。|
|[创建 roleScopeTag](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|创建新的 [roleScopeTag](../resources/intune-rbac-rolescopetag.md) 对象。|
|[删除 roleScopeTag](../api/intune-rbac-rolescopetag-delete.md)|无|删除 [roleScopeTag](../resources/intune-rbac-rolescopetag.md)。|
|[更新 roleScopeTag](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|更新 [roleScopeTag](../resources/intune-rbac-rolescopetag.md) 对象的属性。|
|[分配操作](../api/intune-rbac-rolescopetag-assign.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 集合|尚未记录|
|[getRoleScopeTagsById 操作](../api/intune-rbac-rolescopetag-getrolescopetagsbyid.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) 集合|尚未记录|
|[hasCustomRoleScopeTag 函数](../api/intune-rbac-rolescopetag-hascustomrolescopetag.md)|Boolean|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 此为只读，且自动生成。|
|displayName|String|角色范围标记的显示名称或友好名称。|
|description|String|角色范围标记的说明。|
|isBuiltIn|Boolean|角色范围标记的说明。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 集合|此角色作用域标记的分配列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isBuiltIn": true
}
```






