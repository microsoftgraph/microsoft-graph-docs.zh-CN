---
title: 列出约会
description: 获取指定 bookingBusiness 的 bookingAppointment 对象列表。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: fbb01079dde03e2926775eb16fa6d7f7b972167a
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856048"
---
# <a name="list-appointments"></a>列出约会

命名空间：microsoft.graph

获取指定 [bookingBusiness](../resources/bookingbusiness.md) 的 [bookingAppointment](../resources/bookingappointment.md) 对象列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | BookingsAppointment.ReadWrite.All、Bookings.Read.All   |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /solutions/bookingBusinesses/{id}/appointments
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持$count和$expand [OData 查询参数](/graph/query-parameters) ，以帮助自定义响应。

若要获取日期范围内Microsoft Bookings企业的约会集，而不是`$filter`获取该日期范围[的 calendarView](bookingbusiness-list-calendarview.md)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization  | 持有者 {code}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [bookingAppointment](../resources/bookingappointment.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments
```

### <a name="response"></a>响应

下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses('Contosolunchdelivery%40contoso.onmicrosoft.com')/appointments",
    "value": [
        {
            "id": "AAMkADKoAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "isLocationOnline": true,
            "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MTlhZTE3MDUtODk0Yy00MGZkLTlhNzktN2FmYTk3MDUxNmE2%40thread.v2/0?context=%7b%22Tid%22%3a%22995fa18c-b557-4694-8d07-b89779d6dc77%22%2c%22Oid%22%3a%22d4d260ab-989d-490e-b121-e2066391807a%22%7d",
            "customers": [
                {
                    "@odata.type": "#microsoft.graph.bookingCustomerInformation",
                    "customerId": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
                    "name": "Bob Kelly",
                    "emailAddress": "bobk@tailspintoys.com",
                    "phone": "213-555-0108",
                    "notes": null,
                    "location": {
                        "displayName": "Customer",
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
                    "timeZone": "America/Chicago"
                }
            ],
            "customerTimeZone": "America/Chicago",
            "smsNotificationsEnabled": true,
            "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "serviceName": "Catered bento",
            "duration": "PT30M",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "priceType": "fixedPrice",
            "price": 10,
            "serviceNotes": null,
            "optOutOfCustomerEmail": false,
            "staffMemberIds": [],
            "startDateTime": {
                "dateTime": "2018-04-30T13:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "endDateTime": {
                "dateTime": "2018-04-30T13:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (987 Third Avenue, Buffalo, NY 98052, USA)",
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
            "reminders": []
        },
        {
            "id": "AAMkADKnAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "isLocationOnline": true,
            "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MDUtODk0Yy00MGZkLTlhNzktN2xNmE2%40thread.v2/0?context=%7b%22Tid%22%3a%22995fa18c-b557-4694-8d07-b89779d6dc77%22%2c%22Oid%22%3a%22d4d260ab-989d-490e-b121-e2066391807a%22%7d",
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
                        "displayName": "Customer",
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
            ],
            "customerTimeZone": "America/Chicago",
            "smsNotificationsEnabled": true,
            "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "serviceName": "Catered bento",
            "duration": "PT30M",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "priceType": "fixedPrice",
            "price": 10,
            "serviceNotes": null,
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
            "reminders": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appointments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
