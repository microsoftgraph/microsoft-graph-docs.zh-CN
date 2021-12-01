---
title: connectedOrganizationMembers 复杂类型
description: connectedOrganizationMembers 类型标识租户中将允许其成为请求者、审批者或审阅者的用户的集合。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eb5fce001b0a1e202d0b8f7b1a7f294208e812c1
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242385"
---
# <a name="connectedorganizationmembers-complex-type"></a>connectedOrganizationMembers 复杂类型

命名空间：microsoft.graph


在访问包分配策略的请求设置中使用。 值指示此类型标识用户的集合，即与已连接组织关联的用户，将允许这些用户 `@odata.type` `#microsoft.graph.connectedOrganizationMembers` 请求访问包。 [](connectedorganization.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|connectedOrganizationId|String|权利管理 [中连接的组织的](connectedorganization.md) ID。|
|description|String|已连接组织的名称。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectedOrganizationMembers",
  "connectedOrganizationId": "String",
  "description": "String"
}
```



