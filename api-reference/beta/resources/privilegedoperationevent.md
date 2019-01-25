---
title: privilegedOperationEvent 资源类型
description: 代表审核事件生成的特权身份管理角色操作，如，管理员可以管理特权的角色、 用户激活其角色，以及用户停用其角色。
localization_priority: Normal
ms.openlocfilehash: 2ad8f7e5db956dfbb2fa0d74f441b01f2b5d68aa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525589"
---
# <a name="privilegedoperationevent-resource-type"></a>privilegedOperationEvent 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表审核事件生成的特权身份管理角色操作，如，管理员可以管理特权的角色、 用户激活其角色，以及用户停用其角色。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md)集合。 |获取 privilegedOperationEvent 对象的集合。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|additionalInformation|string|事件的详细人力易读信息。|
|creationDateTime|dateTimeOffset|指示何时创建该事件的时间。|
|expirationDateTime|dateTimeOffset|仅当 requestType 是"激活"，并指明角色激活的过期时间时，才使用此选项。|
|id|string|PrivilegedOperationEvent 唯一标识符。 只读。|
|referenceKey|string|事件/请求票证角色在激活过程中的编号。 仅当票证次数提供角色激活期间，将显示值。|
|referenceSystem|string|事件/请求票证 tole 激活期间提供的系统。 仅当票证系统提供角色激活期间，将显示值。|
|RequestType|string|请求操作类型。 RequestType 值可以是： ```Assign``` （工作分配角色）， ```Activate``` （角色激活）， ```Unassign``` （删除角色分配，请） ```Deactivate``` （角色停用） ```ScanAlersNow``` （扫描安全警报）， ```DismissAlert``` （消除安全警报）， ```FixAlertItem``` （解决安全通知问题）， ```AccessReview_Review``` （查看访问检查）， ```AccessReview_Create``` （创建访问检查）， ```AccessReview_Update``` （更新访问查看） 和```AccessReview_Delete```（删除访问查看）。|
|requestorId|string|请求者发起操作的用户 id。|
|requestorName|string|发起操作请求者的用户名。|
|roleId|string|与操作相关联的角色的 id。|
|roleName|string|角色的名称。|
|tenantId|string|（组织） 租户 id。|
|userId|string|与操作关联的用户 id。|
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
  "userName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedoperationevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
