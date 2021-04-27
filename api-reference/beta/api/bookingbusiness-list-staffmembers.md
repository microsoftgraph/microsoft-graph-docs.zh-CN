---
title: 列出 staffMembers
description: 获取指定 bookingbusiness 中的 bookingStaffMember 对象列表。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 32fd259d2ac7be2f8fbf9f7b2eda10ff13699315
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047873"
---
# <a name="list-staffmembers"></a><span data-ttu-id="53819-103">列出 staffMembers</span><span class="sxs-lookup"><span data-stu-id="53819-103">List staffMembers</span></span>

<span data-ttu-id="53819-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53819-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53819-105">获取指定的[bookingbusiness](../resources/bookingbusiness.md)[中的 bookingStaffMember](../resources/bookingstaffmember.md)对象列表。</span><span class="sxs-lookup"><span data-stu-id="53819-105">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="53819-106">权限</span><span class="sxs-lookup"><span data-stu-id="53819-106">Permissions</span></span>
<span data-ttu-id="53819-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53819-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53819-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="53819-109">Permission type</span></span>      | <span data-ttu-id="53819-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53819-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53819-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53819-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="53819-112">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="53819-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="53819-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53819-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53819-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="53819-114">Not supported.</span></span>   |
|<span data-ttu-id="53819-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="53819-115">Application</span></span> | <span data-ttu-id="53819-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53819-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="53819-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53819-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53819-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53819-118">Optional query parameters</span></span>
<span data-ttu-id="53819-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="53819-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53819-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="53819-120">Request headers</span></span>
| <span data-ttu-id="53819-121">名称</span><span class="sxs-lookup"><span data-stu-id="53819-121">Name</span></span>      |<span data-ttu-id="53819-122">说明</span><span class="sxs-lookup"><span data-stu-id="53819-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="53819-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53819-123">Authorization</span></span>  | <span data-ttu-id="53819-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="53819-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="53819-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="53819-125">Request body</span></span>
<span data-ttu-id="53819-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53819-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="53819-127">响应</span><span class="sxs-lookup"><span data-stu-id="53819-127">Response</span></span>
<span data-ttu-id="53819-128">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [bookingStaffMember](../resources/bookingstaffmember.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="53819-128">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53819-129">示例</span><span class="sxs-lookup"><span data-stu-id="53819-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53819-130">请求</span><span class="sxs-lookup"><span data-stu-id="53819-130">Request</span></span>
<span data-ttu-id="53819-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53819-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53819-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="53819-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
# <a name="c"></a>[<span data-ttu-id="53819-133">C#</span><span class="sxs-lookup"><span data-stu-id="53819-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-staffmembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53819-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53819-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-staffmembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53819-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53819-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-staffmembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53819-136">Java</span><span class="sxs-lookup"><span data-stu-id="53819-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-staffmembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="53819-137">响应</span><span class="sxs-lookup"><span data-stu-id="53819-137">Response</span></span>
<span data-ttu-id="53819-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53819-138">The following is an example of the response.</span></span> <span data-ttu-id="53819-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53819-139">Note: The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->
