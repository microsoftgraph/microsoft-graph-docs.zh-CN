---
title: 创建 bookingAppointment
description: 为指定的 bookingbusiness 创建新的 bookingAppointment。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 0262ab76e127f2104bdf2edc2e896b8f4a2873b8
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014220"
---
# <a name="create-bookingappointment"></a>创建 bookingAppointment

命名空间：microsoft.graph

为指定的[bookingBusiness](../resources/bookingbusiness.md)创建新的[bookingAppointment。](../resources/bookingappointment.md)
## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | 不支持。  |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /solutions/bookingBusinesses/{id}/appointments

```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {code}。 必需。|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [bookingAppointment](../resources/bookingappointment.md) 对象的 JSON 表示形式。


## <a name="response"></a>响应
如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [bookingAppointment](../resources/bookingappointment.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。 此约会不涉及预订特定员工。

<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.bookingAppointment",
    "customerTimeZone": "America/Chicago",
    "smsNotificationsEnabled": true,
    "endDateTime": {
        "@odata.type": "#microsoft.graph.dateTimeTimeZone",
        "dateTime": "2018-05-01T12:30:00.0000000+00:00",
        "timeZone": "UTC"
    },
    "isLocationOnline": true,
    "optOutOfCustomerEmail": false,
    "postBuffer": "PT10M",
    "preBuffer": "PT5M",
    "price": 10.0,
    "priceType@odata.type": "#microsoft.graph.bookingPriceType",
    "priceType": "fixedPrice",
    "reminders@odata.type": "#Collection(microsoft.graph.bookingReminder)",
    "reminders": [
        {
            "@odata.type": "#microsoft.graph.bookingReminder",
            "message": "This service is tomorrow",
            "offset": "P1D",
            "recipients@odata.type": "#microsoft.graph.bookingReminderRecipients",
            "recipients": "allAttendees"
        },
        {
            "@odata.type": "#microsoft.graph.bookingReminder",
            "message": "Please be available to enjoy your lunch service.",
            "offset": "PT1H",
            "recipients@odata.type": "#microsoft.graph.bookingReminderRecipients",
            "recipients": "customer"
        },
        {
            "@odata.type": "#microsoft.graph.bookingReminder",
            "message": "Please check traffic for next cater.",
            "offset": "PT2H",
            "recipients@odata.type": "#microsoft.graph.bookingReminderRecipients",
            "recipients": "staff"
        }
    ],
    "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceLocation": {
        "@odata.type": "#microsoft.graph.location",
        "address": {
            "@odata.type": "#microsoft.graph.physicalAddress",
            "city": "Buffalo",
            "countryOrRegion": "USA",
            "postalCode": "98052",
            "postOfficeBox": null,
            "state": "NY",
            "street": "123 First Avenue",
            "type@odata.type": "#microsoft.graph.physicalAddressType",
            "type": null
        },
        "coordinates": null,
        "displayName": "Customer location",
        "locationEmailAddress": null,
        "locationType@odata.type": "#microsoft.graph.locationType",
        "locationType": null,
        "locationUri": null,
        "uniqueId": null,
        "uniqueIdType@odata.type": "#microsoft.graph.locationUniqueIdType",
        "uniqueIdType": null
    },
    "serviceName": "Catered bento",
    "serviceNotes": "Customer requires punctual service.",
    "startDateTime": {
        "@odata.type": "#microsoft.graph.dateTimeTimeZone",
        "dateTime": "2018-05-01T12:00:00.0000000+00:00",
        "timeZone": "UTC"
    },
    "maximumAttendeesCount": 5,
    "filledAttendeesCount": 1,
    "customers@odata.type": "#Collection(microsoft.graph.bookingCustomerInformation)",
    "customers": [
        {
            "@odata.type": "#microsoft.graph.bookingCustomerInformation",
            "customerId": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "name": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com",
            "phone": "213-555-0199",
            "notes": null,
            "location": {
                "@odata.type": "#microsoft.graph.location",
                "displayName": "Customer",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "@odata.type": "#microsoft.graph.physicalAddress",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "timeZone":"America/Chicago",
            "customQuestionAnswers": [
                {
                    "questionId": "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
                    "question": "What is your age?",
                    "answerInputType": "text",
                    "answerOptions": [],
                    "isRequired": true,
                    "answer": "25",
                    "selectedOptions": []
                }
            ]
        }
    ]
}
```

### <a name="response"></a>响应
下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses('Contosolunchdelivery%40contoso.onmicrosoft.com')/appointments/$entity",
    "id": "AAMkADc7zF4J0AAA8v_KnAAA=",
    "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
    "isLocationOnline": true,
    "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MTlhZTE3MDUtODk0Yy00MGZkLTlhNzktN2FmYTk3MDUxNmE2%40thread.v2/0?context=%7b%22Tid%22%3a%22995fa18c-b557-4694-8d07-b89779d6dc77%22%2c%22Oid%22%3a%22d4d260ab-989d-490e-b121-e2066391807a%22%7d",
    "smsNotificationsEnabled": true,
    "customerTimeZone": "America/Chicago",
    "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceName": "Catered bento",
    "duration": "PT30M",
    "preBuffer": "PT5M",
    "postBuffer": "PT10M",
    "priceType": "fixedPrice",
    "price": 10,
    "serviceNotes": "Customer requires punctual service.",
    "optOutOfCustomerEmail": false,
    "staffMemberIds": [],
    "startDateTime": {
        "dateTime": "2018-05-01T12:00:00.0000000Z",
        "timeZone": "UTC"
    },
    "endDateTime": {
        "dateTime": "2018-05-01T12:30:00.0000000Z",
        "timeZone": "UTC"
    },
    "serviceLocation": {
        "displayName": "Customer location (123 First Avenue, Buffalo, NY 98052, USA)",
        "locationEmailAddress": null,
        "locationUri": "",
        "locationType": null,
        "uniqueId": null,
        "uniqueIdType": null,
        "address": {
            "street": "",
            "city": "",
            "state": "",
            "countryOrRegion": "",
            "postalCode": ""
        },
        "coordinates": {
            "altitude": null,
            "latitude": null,
            "longitude": null,
            "accuracy": null,
            "altitudeAccuracy": null
        }
    },
    "reminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "This service is tomorrow"
        },
        {
            "offset": "PT1H",
            "recipients": "customer",
            "message": "Please be available to enjoy your lunch service."
        },
        {
            "offset": "PT2H",
            "recipients": "staff",
            "message": "Please check traffic for next cater."
        }
    ],
    "maximumAttendeesCount": 5,
    "filledAttendeesCount": 1,
    "customers": [
        {
            "@odata.type": "#microsoft.graph.bookingCustomerInformation",
            "customerId": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "name": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com",
            "phone": "213-555-0199",
            "notes": null,
            "location": {
                "@odata.type": "#microsoft.graph.location",
                "displayName": "Customer",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "@odata.type": "#microsoft.graph.physicalAddress",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "timeZone": "America/Chicago",
            "customQuestionAnswers": [
                {
                    "questionId": "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
                    "question": "What is your age?",
                    "answerInputType": "text",
                    "answerOptions": [],
                    "isRequired": true,
                    "answer": "25",
                    "selectedOptions": []
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


