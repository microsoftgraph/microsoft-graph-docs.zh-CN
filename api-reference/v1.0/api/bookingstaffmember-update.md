---
title: 更新 bookingStaffMember
description: 更新指定 bookingBusiness 中的 bookingStaffMember 的属性。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e0101a297b48a64fa38d494e53a1315011bfcf0f
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526501"
---
# <a name="update-bookingstaffmember"></a>更新 bookingstaffmember

命名空间：microsoft.graph

更新指定的[bookingBusiness](../resources/bookingbusiness.md)[中的 bookingStaffMember](../resources/bookingstaffmember.md)的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Bookings.ReadWrite.All、Bookings.Manage.All   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | 不支持。  |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {code}。 必需。|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Boolean|True 表示如果员工是 Microsoft 365用户，Microsoft Bookings API 将使用 Microsoft 365 中的员工个人日历以及 **workingHours** 属性来确定可用性。 |
|displayName|String|显示给客户的员工的姓名。|
|emailAddress|String|员工成员的电子邮件地址。 它可以与企业Microsoft 365租户中，也可以在不同的电子邮件域中。 如果在业务的计划策略中将 **sendConfirmationsToOwner** 属性设置为 ，则 `true` 使用此电子邮件地址。|
|role|string| 员工在业务中的角色。 可取值为：`guest`、`administrator`、`viewer`、`externalGuest`。|
|timeZone|字符串|员工员工的时区。 有关可能值的列表，请参阅 [dateTimeTimeZone](../resources/datetimetimezone.md)。|
|useBusinessHours|布尔值|True 表示员工的可用性由业务的业务 **Hours** 属性确定。 False 表示可用性由员工的 **workingHouse** 属性设置确定。|
|workingHours|[bookingWorkHours](../resources/bookingworkhours.md) 集合|一周中每个员工可以预订的小时数范围。|

## <a name="response"></a>响应
如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。
## <a name="example"></a>示例
### <a name="request"></a>请求
以下示例将员工的计划更改为周一关闭。

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingStaffMember",
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[

            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"tuesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "endTime":"17:00:00.0000000",
                    "startTime":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"wednesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "endTime":"17:00:00.0000000",
                    "startTime":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"thursday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "endTime":"17:00:00.0000000",
                    "startTime":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"friday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "endTime":"17:00:00.0000000",
                    "startTime":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```

### <a name="response"></a>响应
下面展示了示例响应。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


