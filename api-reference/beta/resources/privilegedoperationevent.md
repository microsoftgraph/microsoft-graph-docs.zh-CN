---
title: privilegedOperationEvent 资源类型
description: 表示由角色操作的特权标识管理生成的审核事件，例如管理员管理特权角色、用户激活他的角色，以及用户停用他的角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 921fa2068d152652b41f36b8893859df7696b5a8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521521"
---
# <a name="privilegedoperationevent-resource-type"></a>privilegedOperationEvent 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示由角色操作的特权标识管理生成的审核事件，例如管理员管理特权角色、用户激活他的角色，以及用户停用他的角色。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md)集合。 |获取 privilegedOperationEvent 对象的集合。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|additionalInformation|string|事件的详细人员可读信息。|
|creationDateTime|dateTimeOffset|指示创建事件的时间。|
|expirationDateTime|dateTimeOffset|仅当 requestType 为 "Activate" 时才使用此方法，它指示角色激活的过期时间。|
|id|string|PrivilegedOperationEvent 的唯一标识符。 只读。|
|referenceKey|string|角色激活期间的事件/请求票证编号。 仅当在角色激活期间提供了票证号时，才会显示该值。|
|referenceSystem|string|在 tole 激活过程中提供的事件/请求票证发放系统。 仅当在角色激活过程中提供了票证系统时，才会显示该值。|
|requestType|string|请求操作类型。 ```Assign``` RequestType 值可以是：（角色分配）、 ```Activate``` （角色激活）、 ```Unassign``` （删除角色分配```Deactivate``` ）、（角色停用）、 ```ScanAlersNow``` （扫描安全警报）、 ```DismissAlert``` （消除安全警报） ```FixAlertItem``` 、（修复安全警报问题） ```AccessReview_Review``` 、（"查看访问```AccessReview_Create```审核"）、"（创建访问```AccessReview_Update```审核）"、"（删除访问审核）" ```AccessReview_Delete```和 "（删除访问审核）"。|
|requestorId|string|启动操作的请求者的用户 id。|
|requestorName|string|启动操作的请求者的用户名。|
|roleId|string|与操作关联的角色的 id。|
|拥有|string|角色的名称。|
|tenantId|string|租户（组织） id。|
|userId|string|与操作关联的用户的 id。|
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
