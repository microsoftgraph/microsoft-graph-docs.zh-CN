---
title: privilegedOperationEvent 资源类型
description: 表示由Privileged Identity Management为角色操作生成的审核事件，例如管理员管理特权角色、用户激活其角色以及用户停用其角色。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 0002e10cff2324d60f9000b1cdf961b865409056
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397535"
---
# <a name="privilegedoperationevent-resource-type-deprecated"></a>privilegedOperationEvent 资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2AADRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

表示由Privileged Identity Management为角色操作生成的审核事件，例如管理员管理特权角色、用户激活其角色以及用户停用其角色。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md) 集合。 |获取 privilegedOperationEvent 对象的集合。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|additionalInformation|string|事件的详细人类可读信息。|
|creationDateTime|DateTimeOffset|指示创建事件的时间。|
|expirationDateTime|DateTimeOffset|仅当 **requestType** 为 `Activate`requestType 时才使用此值，它指示角色激活的过期时间。|
|id|string|privilegedOperationEvent 的唯一标识符。 只读。|
|referenceKey|string|角色激活期间的事件/请求票证号。 仅当在角色激活期间提供票证号时，才会显示该值。|
|referenceSystem|string|Tole 激活期间提供的事件/请求票证系统。 仅当在角色激活期间提供票证系统时，才会显示该值。|
|requestType|字符串|请求操作类型。 requestType 值可以是： `Assign` (角色分配) ， `Activate` (角色激活) ， `Unassign` (删除角色分配) 、 `Deactivate` (角色停用) 、 `ScanAlertsNow` (扫描安全警报) 、 `DismissAlert` (解除安全警报) 、 `FixAlertItem` (修复安全警报问题) 、  `AccessReview_Review` (查看访问评审) 、 `AccessReview_Create` (创建访问评审) 、 `AccessReview_Update` (更新访问评审) ， `AccessReview_Delete` (删除访问评审) 。|
|requestorId|string|发起操作的请求方的用户 ID。|
|requestorName|string|发起操作的请求方的用户名。|
|roleId|string|与操作关联的角色的 ID。|
|roleName|string|角色的名称。|
|tenantId|string|租户 (组织) ID。|
|userId|string|与操作关联的用户的 ID。|
|userMail|string|用户的电子邮件。|
|userName|string|用户的显示名称。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedOperationEvent"
}-->

```json
{
  "additionalInformation": "string",
  "creationDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "requestType": "string",
  "requestorId": "string",
  "requestorName": "string",
  "roleId": "string",
  "roleName": "string",
  "tenantId": "string",
  "userId": "string",
  "userMail": "string",
  "userName": "string",
  "referenceKey": "string",
  "referenceSystem": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedOperationEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


