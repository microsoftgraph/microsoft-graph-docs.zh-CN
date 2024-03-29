---
title: teamworkTagMember 资源类型
description: 表示团队中应用了标记的用户。
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: b8e6d70a8249168383f2bc1b0e6d8884525855ec
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534514"
---
# <a name="teamworktagmember-resource-type"></a>teamworkTagMember 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示团队中应用了标记的用户。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 teamworkTagMembers](../api/teamworktagmember-list.md)|[**teamworkTagMember**](teamworktagmember.md) 集合|获取团队中标准标记的成员及其属性的列表。|
|[创建 teamworkTagMember](../api/teamworktagmember-post.md)|[**teamworkTagMember**](teamworktagmember.md)|创建新的 **teamworkTagMember** 对象。|
|[获取 teamworkTagMember](../api/teamworktagmember-get.md)|[**teamworkTagMember**](teamworktagmember.md)|获取团队中标准标记的成员的属性和关系。|
|[删除 teamworkTagMember](../api/teamworktagmember-delete.md)|无|从团队中的标准标记中删除成员。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|成员显示名称。|
|ID|String|成员 ID。|
|tenantID|String|标记成员是其中一部分的租户的 ID。|
|userID|String|成员的用户 ID。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "ID",
  "@odata.type": "microsoft.graph.teamworkTagMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagMember",
  "ID": "String (Identifier)",
  "displayName": "String",
  "tenantID": "String",
  "userID": "String"
}
```

