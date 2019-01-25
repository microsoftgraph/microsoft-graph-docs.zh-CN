---
title: bookingStaffMember 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 72130f46dc67d4491f9855706528ee5894b8352f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520275"
---
# <a name="bookingstaffmember-resource-type"></a>bookingStaffMember 资源类型

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
代表一个人员成员提供[bookingBusiness](bookingbusiness.md)中的服务。

员工可以是其中配置预订业务，或者他们可使用其他电子邮件提供程序的电子邮件服务的 Office 355 租户的一部分。

当预订约会，预订 API 考虑以下设置来确定名员工的可用性： 

1. 默认情况下，业务 （ [bookingBusiness](bookingbusiness.md)实体的**工作时间**属性） 的营业时间表示员工成员的常规可用性。
2. 如果**useBusinessHours**为 false，则员工成员的特定工作小时 （ **bookingStaffmember**实体**workingHours**属性） 表示该成员的常规可用性。
3. 如果**availabilityIsAffectedByPersonalCalendar**为 true，然后预订 API 将首先查看员工成员的通常可用时间 （作为由 #1 或 #2），并验证可用性中员工成员的个人这些时间在进行预订之前的日历。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表员工成员](../api/bookingbusiness-list-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md)集合 | 指定[bookingbusiness](../resources/bookingbusiness.md)中获取**bookingStaffMember**对象的列表。 |
|[创建 bookingStaff](../api/bookingbusiness-post-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md)集合 | 在指定[bookingbusiness](../resources/bookingbusiness.md)中创建新**bookingStaffMember** 。 |
|[获取 bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |指定[bookingbusiness](../resources/bookingbusiness.md)中获取的属性和**bookingStaffMember**的关系。|
|[Update](../api/bookingstaffmember-update.md) | [bookingStaffMember](bookingstaffmember.md)    |更新在指定[bookingbusiness](../resources/bookingbusiness.md) **bookingStaffMember**的属性。|
|[删除](../api/bookingstaffmember-delete.md) | 无 |删除指定[bookingbusiness](../resources/bookingbusiness.md)中的人员成员。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Boolean|True 表示，如果该人员成员是 Office 365 用户，预订 API 将验证员工成员的可用性其 Office 365 中的个人日历中之前进行预订。 |
|ColorIndex|Int32|标识要表示员工成员的颜色。 颜色对应于预订应用程序中的**人员详细信息**页面中的调色板。|
|displayName|String|员工成员，显示给客户的名称。 必需。|
|emailAddress|String|员工成员的电子邮件地址。 这可以随着业务，相同的 Office 365 租户中或不同的电子邮件域中。 可使用此电子邮件地址，如果**sendConfirmationsToOwner**属性设置为 true 的企业计划策略。 必需。|
|id|字符串| 员工成员，GUID 格式的 ID。 只读。|
|role|string| 企业中的人员成员角色。 可取值为：`guest`、`administrator`、`viewer`、`externalGuest`。 必需。|
|useBusinessHours|Boolean|True 的表示员工成员的可用性，作为业务**businessHours**属性中指定。 False，则意味着可用性由员工成员的**workingHours**属性设置。|
|workingHours|[bookingWorkHours](bookingworkhours.md)集合|员工成员了可供预定的一周中每一天时间范围。 默认情况下，它们都初始化为业务的**工作时间**属性相同。|

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
  "role": "string",
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}]
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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingstaffmember.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
