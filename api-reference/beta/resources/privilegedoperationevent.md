---
title: privilegedOperationEvent 资源类型
description: 表示由 Privileged Identity Management 为角色操作生成的审核事件，例如管理员管理特权角色、用户激活其角色以及用户停用其角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 408eb2ca06168b4e22b945aa9d3d6faa2b1a561a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440142"
---
# <a name="privilegedoperationevent-resource-type"></a>privilegedOperationEvent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示由 Privileged Identity Management 为角色操作生成的审核事件，例如管理员管理特权角色、用户激活其角色以及用户停用其角色。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md) 集合。 |获取 privilegedOperationEvent 对象的集合。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|additionalInformation|string|事件的详细人工可读信息。|
|creationDateTime|dateTimeOffset|指示创建事件的时间。|
|expirationDateTime|dateTimeOffset|This is only used when the requestType is "Activate"， and it indicates the expiration time for the role activation.|
|id|string|privilegedOperationEvent 的唯一标识符。 只读。|
|referenceKey|string|角色激活期间的事件/请求票证编号。 该值仅在角色激活期间提供票证编号时显示。|
|referenceSystem|string|Tole 激活期间提供的事件/请求票证系统。 该值仅在角色激活期间提供票证系统时显示。|
|requestType|string|请求操作类型。 requestType 值可以是： (角色分配)  (```Assign``` ```Activate``` 激活) ， (删除角色分配) ， (角色停用) 、 (扫描安全警报) 、 (消除安全警报) 、 (修复安全警报问题 ```Unassign``` ```Deactivate``` ```ScanAlersNow```) 、 (查看访问评审 ```DismissAlert``` ```FixAlertItem```) 、 (创建访问评审 ```AccessReview_Review``` ```AccessReview_Create```) 、 (```AccessReview_Update``` 更新 ```AccessReview_Delete``` 访问评审) 和 (删除访问评审) 。|
|requestorId|string|启动该操作的请求者的用户 ID。|
|requestorName|string|启动该操作的请求者用户名。|
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


