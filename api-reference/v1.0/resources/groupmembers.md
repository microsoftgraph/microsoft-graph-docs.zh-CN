---
title: groupMembers 复杂类型
description: 标识租户中将允许其成为请求者、审批者或审阅者的用户的集合。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 18260b0b94ddc50e60e60f427e0e4f879912758d
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242347"
---
# <a name="groupmembers-complex-type"></a>groupMembers 复杂类型

命名空间：microsoft.graph


在访问包分配策略的请求、审批和分配审阅设置中使用。
该值指示此类型标识租户中将允许作为请求者、审批者或审阅者的用户集合，这些用户是特定 `@odata.type` `#microsoft.graph.groupMembers` 组的成员。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|组中组的名称Azure AD。 只读。 |
|groupId|String|组中[组的](group.md)ID Azure AD。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupMembers",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupMembers",
  "groupId": "String",
  "description": "String"
}
```



