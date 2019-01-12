---
title: 列表 staffMembers
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 81f170e101ad2aa600991cb79eaccdc65db8e4be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951381"
---
# <a name="list-staffmembers"></a><span data-ttu-id="bc096-104">列表 staffMembers</span><span class="sxs-lookup"><span data-stu-id="bc096-104">List staffMembers</span></span>

 > <span data-ttu-id="bc096-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bc096-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc096-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc096-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="bc096-107">指定[bookingbusiness](../resources/bookingbusiness.md)中获取[bookingStaffMember](../resources/bookingstaffmember.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="bc096-107">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="bc096-108">权限</span><span class="sxs-lookup"><span data-stu-id="bc096-108">Permissions</span></span>
<span data-ttu-id="bc096-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc096-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc096-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc096-111">Permission type</span></span>      | <span data-ttu-id="bc096-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc096-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc096-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc096-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="bc096-114">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="bc096-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="bc096-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc096-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc096-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc096-116">Not supported.</span></span>   |
|<span data-ttu-id="bc096-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc096-117">Application</span></span> | <span data-ttu-id="bc096-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc096-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bc096-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc096-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bc096-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bc096-120">Optional query parameters</span></span>
<span data-ttu-id="bc096-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bc096-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc096-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc096-122">Request headers</span></span>
| <span data-ttu-id="bc096-123">名称</span><span class="sxs-lookup"><span data-stu-id="bc096-123">Name</span></span>      |<span data-ttu-id="bc096-124">说明</span><span class="sxs-lookup"><span data-stu-id="bc096-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc096-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc096-125">Authorization</span></span>  | <span data-ttu-id="bc096-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bc096-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc096-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc096-127">Request body</span></span>
<span data-ttu-id="bc096-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bc096-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bc096-129">响应</span><span class="sxs-lookup"><span data-stu-id="bc096-129">Response</span></span>
<span data-ttu-id="bc096-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[bookingStaffMember](../resources/bookingstaffmember.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="bc096-130">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc096-131">示例</span><span class="sxs-lookup"><span data-stu-id="bc096-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc096-132">请求</span><span class="sxs-lookup"><span data-stu-id="bc096-132">Request</span></span>
<span data-ttu-id="bc096-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bc096-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
##### <a name="response"></a><span data-ttu-id="bc096-134">响应</span><span class="sxs-lookup"><span data-stu-id="bc096-134">Response</span></span>
<span data-ttu-id="bc096-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bc096-135">The following is an example of the response.</span></span> <span data-ttu-id="bc096-136">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bc096-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bc096-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc096-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers",
    "value":[
        {
            "id":"8ee1c803-a1fa-406d-8259-7ab53233f148",
            "displayName":"Dana Swope",
            "emailAddress":"danas@contoso.com",
            "availabilityIsAffectedByPersonalCalendar":false,
            "colorIndex":1,
            "role":"externalGuest",
            "useBusinessHours":true,
            "workingHours":[
                {
                    "day":"monday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"tuesday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"wednesday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"thursday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"friday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                }
            ]
        },
        {
            "id":"71d64d0e-7225-49b6-b0b1-070d476cda51",
            "displayName":"Samantha Booth",
            "emailAddress":"samanthab@M365B489948.OnMicrosoft.com",
            "availabilityIsAffectedByPersonalCalendar":true,
            "colorIndex":0,
            "role":"administrator",
            "useBusinessHours":true,
            "workingHours":[
                {
                    "day":"monday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"tuesday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"wednesday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"thursday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"friday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"saturday",
                    "timeSlots":[

                    ]
                },
                {
                    "day":"sunday",
                    "timeSlots":[

                    ]
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List staffMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
