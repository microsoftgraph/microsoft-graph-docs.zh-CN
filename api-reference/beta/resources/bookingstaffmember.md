---
title: bookingStaffMember 资源类型
description: 表示在 bookingBusiness 中提供服务的员工。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 1763191ae18be8ac5c77a40727ea38f388326648
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524887"
---
# <a name="bookingstaffmember-resource-type"></a>bookingStaffMember 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示在 [bookingBusiness 中提供服务的员工](bookingbusiness.md)。

员工可以是配置预订Microsoft 365租户的一部分，或者可以使用其他电子邮件提供商的电子邮件服务。

预订约会时，Bookings API 会考虑以下设置来确定员工是否可用： 

1. 默认情况下 [，bookingBusiness](bookingbusiness.md)实体 (**businessHours** 属性的工作时间) 表示员工常规的可用时间。
2. 如果 **useBusinessHours** 为 false，则 **bookingStaffmember** 实体 (员工的特定工作时间 (**workingHours** 属性表示该成员) 的常规可用性。
3. 如果 **availabilityIsAffectedByPersonalCalendar** 为 true，则 Bookings API 将首先查看由 #1 或 #2) 确定的员工的通常可用小时数 (，并验证这些时段在员工的个人日历中的可用性，然后再进行预订。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出员工](../api/bookingbusiness-list-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md) 集合 | 获取指定的 [bookingbusiness](../resources/bookingbusiness.md)中的 **bookingStaffMember** 对象列表。 |
|[创建 bookingStaff](../api/bookingbusiness-post-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md) 集合 | 在指定的 [bookingbusiness](../resources/bookingbusiness.md)中创建新的 **bookingStaffMember。** |
|[获取 bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |获取指定的 bookingbusiness **中的 bookingStaffMember** [的属性和关系](../resources/bookingbusiness.md)。|
|[更新](../api/bookingstaffmember-update.md) | [bookingStaffMember](bookingstaffmember.md)    |更新指定的 [bookingbusiness](../resources/bookingbusiness.md)**中的 bookingStaffMember** 的属性。|
|[删除](../api/bookingstaffmember-delete.md) | 无 |删除指定 [bookingbusiness 中的员工](../resources/bookingbusiness.md)。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Boolean|True 表示如果员工是 Microsoft 365用户，Bookings API 将验证员工能否在 Microsoft 365 个人日历中，然后再进行预订。 |
|colorIndex|Int32|标识表示员工成员的颜色。 颜色对应于 Bookings 应用中"员工 **详细信息** "页中的调色板。|
|displayName|String|显示给客户的员工的姓名。 必填。|
|emailAddress|String|员工成员的电子邮件地址。 它可以与企业Microsoft 365租户中，也可以在不同的电子邮件域中。 如果在业务的计划策略中 **将 sendConfirmationsToOwner** 属性设置为 true，可以使用此电子邮件地址。 必需。|
|id|String| 采用 GUID 格式的员工 ID。 只读。|
|role|bookingStaffRole| 员工在业务中的角色。 可能的值是 `guest` `administrator` ：、、 `viewer` `externalGuest` 和 `unknownFutureValue` 。 必填。|
|timeZone|字符串|员工员工的时区。 有关可能值的列表，请参阅 [dateTimeTimeZone](datetimetimezone.md)。|
|useBusinessHours|布尔值|True 表示员工的可用性是业务 **businessHours** 属性中指定的。 False 表示可用性由员工的 **workingHours** 属性设置确定。|
|workingHours|[bookingWorkHours](bookingworkhours.md) 集合|一周中每个员工可以预订的小时数范围。 默认情况下，它们初始化为与业务的业务 **Hours** 属性相同。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingStaffMember"
}-->

```json
{
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "role": {"@odata.type": "microsoft.graph.bookingStaffRole"},
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}],
  "timeZone": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


