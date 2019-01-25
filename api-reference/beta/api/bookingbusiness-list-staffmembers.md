---
title: 列表 staffMembers
description: 指定 bookingbusiness 中获取 bookingStaffMember 对象的列表。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 4d8cfcfcab5478149404f4ac990ab45aa0d61c1c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527547"
---
# <a name="list-staffmembers"></a><span data-ttu-id="3cdb4-103">列表 staffMembers</span><span class="sxs-lookup"><span data-stu-id="3cdb4-103">List staffMembers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cdb4-104">指定[bookingbusiness](../resources/bookingbusiness.md)中获取[bookingStaffMember](../resources/bookingstaffmember.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3cdb4-104">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3cdb4-105">权限</span><span class="sxs-lookup"><span data-stu-id="3cdb4-105">Permissions</span></span>
<span data-ttu-id="3cdb4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cdb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cdb4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cdb4-108">Permission type</span></span>      | <span data-ttu-id="3cdb4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cdb4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cdb4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cdb4-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3cdb4-111">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3cdb4-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3cdb4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cdb4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cdb4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cdb4-113">Not supported.</span></span>   |
|<span data-ttu-id="3cdb4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cdb4-114">Application</span></span> | <span data-ttu-id="3cdb4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cdb4-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3cdb4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cdb4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3cdb4-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3cdb4-117">Optional query parameters</span></span>
<span data-ttu-id="3cdb4-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3cdb4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cdb4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cdb4-119">Request headers</span></span>
| <span data-ttu-id="3cdb4-120">名称</span><span class="sxs-lookup"><span data-stu-id="3cdb4-120">Name</span></span>      |<span data-ttu-id="3cdb4-121">说明</span><span class="sxs-lookup"><span data-stu-id="3cdb4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3cdb4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cdb4-122">Authorization</span></span>  | <span data-ttu-id="3cdb4-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3cdb4-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cdb4-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cdb4-124">Request body</span></span>
<span data-ttu-id="3cdb4-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3cdb4-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3cdb4-126">响应</span><span class="sxs-lookup"><span data-stu-id="3cdb4-126">Response</span></span>
<span data-ttu-id="3cdb4-127">如果成功，此方法返回`200 OK`响应代码和响应正文中的[bookingStaffMember](../resources/bookingstaffmember.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="3cdb4-127">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3cdb4-128">示例</span><span class="sxs-lookup"><span data-stu-id="3cdb4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3cdb4-129">请求</span><span class="sxs-lookup"><span data-stu-id="3cdb4-129">Request</span></span>
<span data-ttu-id="3cdb4-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3cdb4-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
##### <a name="response"></a><span data-ttu-id="3cdb4-131">响应</span><span class="sxs-lookup"><span data-stu-id="3cdb4-131">Response</span></span>
<span data-ttu-id="3cdb4-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3cdb4-132">The following is an example of the response.</span></span> <span data-ttu-id="3cdb4-133">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3cdb4-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3cdb4-134">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3cdb4-134">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List staffMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list-staffmembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
