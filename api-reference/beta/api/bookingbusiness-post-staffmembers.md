---
title: 创建 bookingStaffMember
description: 在指定的 bookingbusiness 中创建新的教职员工成员。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 873d0ffa95be5e9dbcf95bbfa95ac942af9b46d7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318259"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="ed388-103">创建 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="ed388-103">Create bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed388-104">在指定的[bookingbusiness](../resources/bookingbusiness.md)中创建新的[教职员工成员](../resources/bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="ed388-104">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ed388-105">权限</span><span class="sxs-lookup"><span data-stu-id="ed388-105">Permissions</span></span>
<span data-ttu-id="ed388-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed388-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed388-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed388-108">Permission type</span></span>      | <span data-ttu-id="ed388-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed388-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed388-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed388-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ed388-111">全部预订. 全部, 全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="ed388-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ed388-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed388-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed388-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed388-113">Not supported.</span></span>   |
|<span data-ttu-id="ed388-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed388-114">Application</span></span> | <span data-ttu-id="ed388-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed388-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ed388-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed388-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="ed388-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed388-117">Request headers</span></span>
| <span data-ttu-id="ed388-118">名称</span><span class="sxs-lookup"><span data-stu-id="ed388-118">Name</span></span>       | <span data-ttu-id="ed388-119">说明</span><span class="sxs-lookup"><span data-stu-id="ed388-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ed388-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed388-120">Authorization</span></span>  | <span data-ttu-id="ed388-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ed388-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed388-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed388-122">Request body</span></span>
<span data-ttu-id="ed388-123">在请求正文中, 提供[bookingStaffMember](../resources/bookingstaffmember.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed388-123">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="ed388-124">您必须包含以下属性:</span><span class="sxs-lookup"><span data-stu-id="ed388-124">You must include the following properties:</span></span>

- <span data-ttu-id="ed388-125">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ed388-125">**displayName**</span></span>
- <span data-ttu-id="ed388-126">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="ed388-126">**emailAddress**</span></span>
- <span data-ttu-id="ed388-127">**role**</span><span class="sxs-lookup"><span data-stu-id="ed388-127">**role**</span></span>


## <a name="response"></a><span data-ttu-id="ed388-128">响应</span><span class="sxs-lookup"><span data-stu-id="ed388-128">Response</span></span>
<span data-ttu-id="ed388-129">如果成功, 此方法在`201, Created`响应正文中返回响应代码和[bookingStaffMember](../resources/bookingstaffmember.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ed388-129">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed388-130">示例</span><span class="sxs-lookup"><span data-stu-id="ed388-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed388-131">请求</span><span class="sxs-lookup"><span data-stu-id="ed388-131">Request</span></span>
<span data-ttu-id="ed388-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed388-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ed388-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ed388-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ed388-134">C#</span><span class="sxs-lookup"><span data-stu-id="ed388-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingstaffmember-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed388-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed388-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingstaffmember-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ed388-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="ed388-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingstaffmember-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ed388-137">Java</span><span class="sxs-lookup"><span data-stu-id="ed388-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingstaffmember-from-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ed388-138">在请求正文中, 提供[bookingStaffMember](../resources/bookingstaffmember.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed388-138">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ed388-139">响应</span><span class="sxs-lookup"><span data-stu-id="ed388-139">Response</span></span>
<span data-ttu-id="ed388-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ed388-140">The following is an example of the response.</span></span> <span data-ttu-id="ed388-141">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ed388-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ed388-142">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ed388-142">All of the properties will be returned from an actual call.</span></span>
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
