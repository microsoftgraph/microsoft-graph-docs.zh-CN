---
title: bookingStaffMember 资源类型
description: 表示在 bookingBusiness 中提供服务的员工。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 25569646633195e9cbce1067dad1abbd369885a2
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160627"
---
# <a name="bookingstaffmember-resource-type"></a>bookingStaffMember 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示在 [bookingBusiness](bookingbusiness.md) 中提供服务的员工。

工作人员可以是配置预订业务Microsoft 365租户的一部分，也可以使用来自其他电子邮件提供商的电子邮件服务。

预订约会时，Bookings API 会考虑以下设置来确定员工的可用性： 

1. 默认情况下，业务运行时间 ([bookingBusiness](bookingbusiness.md) 实体的 **businessHours** 属性) 表示员工的正式发布。
2. 如果 **useBusinessHours** 为 false，则工作人员的特定工作时间 (**bookingStaffmember** 实体的 **workHours** 属性) 表示该成员的正式发布。
3. 如果 **availabilityIsAffectedByPersonalCalendar** 为 true，则 Bookings API 会先查看员工的正式工作时间 (由 #1 或 #2) 确定，然后在员工的个人日历中验证这些时间的可用性，然后再进行预订。

Microsoft Bookings在预订日历中最多支持 100 名工作人员。

## <a name="methods"></a>方法

| 方法           | 返回类型    |Description|
|:---------------|:--------|:----------|
|[列出员工成员](../api/bookingbusiness-list-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md) 集合 | 获取指定 [bookingbusiness](../resources/bookingbusiness.md) 中的 **bookingStaffMember** 对象列表。 |
|[创建 bookingStaff](../api/bookingbusiness-post-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md) 集合 | 在指定的 [bookingbusiness](../resources/bookingbusiness.md) 中创建新的 **bookingStaffMember**。 |
|[获取 bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |获取指定 [bookingbusiness](../resources/bookingbusiness.md) 中 **bookingStaffMember** 的属性和关系。|
|[更新](../api/bookingstaffmember-update.md) | 无   |更新指定 [bookingbusiness](../resources/bookingbusiness.md) 中 **bookingStaffMember** 的属性。|
|[删除](../api/bookingstaffmember-delete.md) | 无 |删除指定 [bookingbusiness](../resources/bookingbusiness.md) 中的员工。 |

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|布尔|True 表示，如果工作人员是Microsoft 365用户，则 Bookings API 会在进行预订之前验证员工在Microsoft 365的个人日历中的可用性。 |
|colorIndex|Int32|标识表示工作人员的颜色。 颜色对应于 Bookings 应用中 **“员工详细信息** ”页中的调色板。|
|displayName|String|向客户显示的工作人员的名称。 必需项。|
|emailAddress|String|工作人员的电子邮件地址。 这可以位于与企业相同的Microsoft 365租户中，也可以位于其他电子邮件域中。 如果在业务的计划策略中 **将 sendConfirmationsToOwner** 属性设置为 true，则可以使用此电子邮件地址。 必需。|
|id|String| 工作人员的 ID，采用 GUID 格式。 只读。|
|IsEmailNotificationEnabled|布尔|`True` 表示在创建或更改分配给他们的预订时，员工成员将通过电子邮件收到通知。
|role|bookingStaffRole| 员工在业务中的角色。 可能的值为：`guest`、`administrator`、`viewer`、`externalGuest`和 `scheduler` `unknownFutureValue``member`。 请注意，必须使用`Prefer: include-unknown-enum-members`请求标头获取以下值 (在此) `[evolvable enum](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`： `scheduler``member` 必需项。 |
|timeZone|String|工作人员的时区。 有关可能值的列表，请参阅 [dateTimeTimeZone](datetimetimezone.md)。|
|useBusinessHours|布尔|True 表示员工的可用性是在企业的 **businessHours** 属性中指定的。 False 表示可用性由工作人员 **的 workingHours** 属性设置确定。|
|workingHours|[bookingWorkHours](bookingworkhours.md) 集合|工作人员可预订的一周中每天的小时数范围。 默认情况下，它们初始化为与企业的 **businessHours** 属性相同。|

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
  "timeZone": "String",
  "IsEmailNotificationEnabled": "Boolean"
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


