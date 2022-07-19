---
title: bookingsBusiness： getStaffAvailability
description: 了解如何获取Microsoft Bookings日历中工作人员的可用性信息。
ms.localizationpriority: medium
author: kwekua
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 07fe80d3fc311c91f1e1b60987a0ebe12f0eda94
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856430"
---
# <a name="bookingsbusiness-getstaffavailability"></a>bookingsBusiness： getStaffAvailability

命名空间：microsoft.graph

获取[Microsoft Bookings日历](../resources/bookingappointment.md)[的工作人员](../resources/bookingstaffmember.md)的可用性信息。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | Calendar.Read、Calendar.ReadWrite、Bookings.Read.All、Calendars.ReadWrite  |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /solutions/bookingBusinesses/{id}/getStaffAvailability
```

## <a name="request-header"></a>请求标头

|名称 |说明 |
|:--------------|:------------|
|Authorization |持有者 {code}。必需。 |
|Content-Type| application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，传递员工 ID 列表以及 [dateTimeTimeZone 资源类型](/graph/resources/datetimetimezone) （称为 **startDateTime** 和 **endDateTime**）的另外两个参数。 这些对应于返回员工可用性的两个时间戳。

## <a name="response"></a>响应

如果成功，此方法会在响应中返回 `200 OK` 响应代码和 [staffAvailabilityItem](../resources/staffavailabilityitem.md) 集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getstaffavailability"
}-->

```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/getStaffAvailability 
Content-Type: application/json

{ 
    "staffIds": [ 
        "311a5454-08b2-4560-ba1c-f715e938cb79" 
    ], 
    "startDateTime": { 
        "dateTime": "2022-01-25T00: 00: 00", 
        "timeZone": "India Standard Time" 
    }, 
    "endDateTime": { 
        "dateTime": "2022-01-26T17: 00: 00", 
        "timeZone": "Pacific Standard Time" 
    } 
}
```

### <a name="response"></a>响应

以下示例显示了相应的响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.staffAvailabilityItem",
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{ 
    "staffAvailabilityItem": [ 
        { 
            "staffId": "311a5454-08b2-4560-ba1c-f715e938cb79", 
            "availabilityItems": [ 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-24T08:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-24T15:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                }, 
                { 
                    "status": "Busy", 
                    "startDateTime": { 
                        "dateTime": "2022-01-24T15:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-24T16:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976" 
                }, 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-24T16:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-24T17:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                }, 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-25T08:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-25T17:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                }, 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-26T08:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-26T17:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                } 
            ] 
        } 
    ] 
}
```
<!-- 
In the response body, for each staff member, their available windows are returned. The types of status of the windows are explained below.
|Type      | Explanation              |
|:--------------------|:---------------------------------------------------------|
|Available | The staff member is available in the given window.   |
|slotAvailable | The staff member has an appointment in the given window. The appointment is for a service which has **maxAttendeecount** more than 1. The customer can join this appointment as there are empty slots available.   |
|Busy | The staff member has an appointment in the given window. Either the staff member has an appointment for a service which has **maxAttendeecount** equal to 1 or the staff has an appointment for a service with **maxAttendeecount** more than 1 but without any available slots.  |
-->