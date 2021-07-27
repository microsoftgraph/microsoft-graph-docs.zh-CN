---
title: teamworkTag 资源类型
description: 表示与团队关联的标记。
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 677ddc348d1cd3ae152d7b777a6b29319839266c
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533897"
---
# <a name="teamworktag-resource-type"></a>teamworkTag 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与团队关联的标记。 

标签为客户提供了一种灵活的方法，可以基于团队中的常见属性对用户或组进行分类。 例如，通过一个"百年"或"经理"或"设计器"标记，用户可以访问 Teams 中的各组人员，而无需键入每个名称。

添加标记后，用户可以在@mention添加标记。 分配了该标记的每个人都将收到通知，就像他们单独接收@mentioned一样。 用户还可使用 标记启动具有该标记成员的新聊天。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出团队合作标记](../api/teamworktag-list.md)|[**teamworkTag**](teamworktag.md) 集合|获取 **teamworkTag 对象** 及其属性的列表。|
|[创建团队合作标记](../api/teamworktag-post.md)|[**teamworkTag**](teamworktag.md)|创建新的 **团队合作标记** 对象。|
|[获取团队合作标记](../api/teamworktag-get.md)|[**teamworkTag**](teamworktag.md)|读取团队合作Tag 对象 **的属性和** 关系。|
|[更新团队合作标记](../api/teamworktag-update.md)|[**teamworkTag**](teamworktag.md)|更新团队合作 **Tag 对象** 的属性。|
|[删除团队合作标记](../api/teamworktag-delete.md)|无|删除 **团队合作标记** 对象。|
|[列出 teamworkTagMembers](../api/teamworktagmember-list.md)|[**teamworkTagMember**](teamworktagmember.md) 集合|获取团队中标准标记的成员及其属性的列表。|
|[创建 teamworkTagMember](../api/teamworktagmember-post.md)|[**teamworkTagMember**](teamworktagmember.md)|创建新的 **teamworkTagMember** 对象。|
|[获取 teamworkTagMember](../api/teamworktagmember-get.md)|[**teamworkTagMember**](teamworktagmember.md)|获取团队中标准标记的成员的属性和关系。|
|[删除 teamworkTagMember](../api/teamworktagmember-delete.md)|无|从团队中的标准标记中删除成员。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|标记说明，因为它将显示在用户Microsoft Teams。|
|displayName|String|标记名称，因为它将显示在用户Microsoft Teams。|
|id|String|标记的 ID。|
|memberCount|Int32|分配给标记的用户数。|
|tagType|teamworkTagType|标记的类型。 默认值为标准。|
|teamId|String|定义标记的团队的 ID。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|成员|[teamworkTagMember](../resources/teamworktagmember.md) 集合|分配给标记的用户。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkTag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "String (identifier)",
  "teamId": "String",
  "displayName": "String",
  "memberCount": "Integer",
  "tagType": "String"
}
```

