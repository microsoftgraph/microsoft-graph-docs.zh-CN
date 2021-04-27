---
title: 创建 bookingStaffMember
description: 在指定的 bookingbusiness 中创建新员工。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e92b3cc416d3cfe462c65da35f8bb4dd6d2e6b50
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047852"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="0a1c0-103">创建 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="0a1c0-103">Create bookingStaffMember</span></span>

<span data-ttu-id="0a1c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a1c0-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a1c0-105">在指定的[bookingbusiness](../resources/bookingstaffmember.md)中创建新的[员工。](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="0a1c0-105">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="0a1c0-106">权限</span><span class="sxs-lookup"><span data-stu-id="0a1c0-106">Permissions</span></span>
<span data-ttu-id="0a1c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a1c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a1c0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a1c0-109">Permission type</span></span>      | <span data-ttu-id="0a1c0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a1c0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a1c0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a1c0-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="0a1c0-112">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0a1c0-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0a1c0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a1c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a1c0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a1c0-114">Not supported.</span></span>   |
|<span data-ttu-id="0a1c0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a1c0-115">Application</span></span> | <span data-ttu-id="0a1c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a1c0-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0a1c0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a1c0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="0a1c0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a1c0-118">Request headers</span></span>
| <span data-ttu-id="0a1c0-119">名称</span><span class="sxs-lookup"><span data-stu-id="0a1c0-119">Name</span></span>       | <span data-ttu-id="0a1c0-120">说明</span><span class="sxs-lookup"><span data-stu-id="0a1c0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0a1c0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a1c0-121">Authorization</span></span>  | <span data-ttu-id="0a1c0-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0a1c0-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a1c0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a1c0-123">Request body</span></span>
<span data-ttu-id="0a1c0-124">在请求正文中，提供 [bookingStaffMember](../resources/bookingstaffmember.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a1c0-124">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="0a1c0-125">必须包括以下属性：</span><span class="sxs-lookup"><span data-stu-id="0a1c0-125">You must include the following properties:</span></span>

- <span data-ttu-id="0a1c0-126">**displayName**</span><span class="sxs-lookup"><span data-stu-id="0a1c0-126">**displayName**</span></span>
- <span data-ttu-id="0a1c0-127">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="0a1c0-127">**emailAddress**</span></span>
- <span data-ttu-id="0a1c0-128">**role**</span><span class="sxs-lookup"><span data-stu-id="0a1c0-128">**role**</span></span>


## <a name="response"></a><span data-ttu-id="0a1c0-129">响应</span><span class="sxs-lookup"><span data-stu-id="0a1c0-129">Response</span></span>
<span data-ttu-id="0a1c0-130">如果成功，此方法在 `201, Created` 响应正文中返回 响应代码和 [bookingStaffMember](../resources/bookingstaffmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0a1c0-130">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a1c0-131">示例</span><span class="sxs-lookup"><span data-stu-id="0a1c0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a1c0-132">请求</span><span class="sxs-lookup"><span data-stu-id="0a1c0-132">Request</span></span>
<span data-ttu-id="0a1c0-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0a1c0-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a1c0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a1c0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookingstaffmember_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Content-type: application/json
Content-length: 309

{
    "@odata.type":"#microsoft.graph.bookingStaffMember",
    "colorIndex":1,
    "displayName":"Dana Swope",
    "emailAddress":"danas@contoso.com",
    "role@odata.type":"#microsoft.graph.bookingStaffRole",
    "role":"externalGuest",
    "useBusinessHours":true,
    "workingHours@odata.type":"#Collection(microsoft.graph.bookingWorkHours)",
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
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
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
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
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
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
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
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
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="0a1c0-135">C#</span><span class="sxs-lookup"><span data-stu-id="0a1c0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingstaffmember-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a1c0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a1c0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingstaffmember-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a1c0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a1c0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingstaffmember-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a1c0-138">Java</span><span class="sxs-lookup"><span data-stu-id="0a1c0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingstaffmember-from-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0a1c0-139">在请求正文中，提供 [bookingStaffMember](../resources/bookingstaffmember.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a1c0-139">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0a1c0-140">响应</span><span class="sxs-lookup"><span data-stu-id="0a1c0-140">Response</span></span>
<span data-ttu-id="0a1c0-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0a1c0-141">The following is an example of the response.</span></span> <span data-ttu-id="0a1c0-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0a1c0-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers/$entity",
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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


