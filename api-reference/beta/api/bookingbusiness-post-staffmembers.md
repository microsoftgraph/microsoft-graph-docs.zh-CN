---
title: 创建 bookingStaffMember
description: 在指定的 bookingbusiness 中创建新的教职员工成员。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9ac0e87e5bf051cb0998d05b361bf5149d5b4e08
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258112"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="ab965-103">创建 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="ab965-103">Create bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab965-104">在指定的[bookingbusiness](../resources/bookingbusiness.md)中创建新的[教职员工成员](../resources/bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="ab965-104">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ab965-105">权限</span><span class="sxs-lookup"><span data-stu-id="ab965-105">Permissions</span></span>
<span data-ttu-id="ab965-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab965-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab965-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab965-108">Permission type</span></span>      | <span data-ttu-id="ab965-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab965-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab965-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab965-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ab965-111">全部预订. 全部, 全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="ab965-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ab965-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab965-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab965-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab965-113">Not supported.</span></span>   |
|<span data-ttu-id="ab965-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab965-114">Application</span></span> | <span data-ttu-id="ab965-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab965-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ab965-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab965-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="ab965-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab965-117">Request headers</span></span>
| <span data-ttu-id="ab965-118">名称</span><span class="sxs-lookup"><span data-stu-id="ab965-118">Name</span></span>       | <span data-ttu-id="ab965-119">说明</span><span class="sxs-lookup"><span data-stu-id="ab965-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab965-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab965-120">Authorization</span></span>  | <span data-ttu-id="ab965-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ab965-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab965-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab965-122">Request body</span></span>
<span data-ttu-id="ab965-123">在请求正文中, 提供[bookingStaffMember](../resources/bookingstaffmember.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab965-123">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="ab965-124">您必须包含以下属性:</span><span class="sxs-lookup"><span data-stu-id="ab965-124">You must include the following properties:</span></span>

- <span data-ttu-id="ab965-125">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ab965-125">**displayName**</span></span>
- <span data-ttu-id="ab965-126">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="ab965-126">**emailAddress**</span></span>
- <span data-ttu-id="ab965-127">**role**</span><span class="sxs-lookup"><span data-stu-id="ab965-127">**role**</span></span>


## <a name="response"></a><span data-ttu-id="ab965-128">响应</span><span class="sxs-lookup"><span data-stu-id="ab965-128">Response</span></span>
<span data-ttu-id="ab965-129">如果成功, 此方法在`201, Created`响应正文中返回响应代码和[bookingStaffMember](../resources/bookingstaffmember.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ab965-129">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab965-130">示例</span><span class="sxs-lookup"><span data-stu-id="ab965-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab965-131">请求</span><span class="sxs-lookup"><span data-stu-id="ab965-131">Request</span></span>
<span data-ttu-id="ab965-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab965-132">The following is an example of the request.</span></span>
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
<span data-ttu-id="ab965-133">在请求正文中, 提供[bookingStaffMember](../resources/bookingstaffmember.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab965-133">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ab965-134">响应</span><span class="sxs-lookup"><span data-stu-id="ab965-134">Response</span></span>
<span data-ttu-id="ab965-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ab965-135">The following is an example of the response.</span></span> <span data-ttu-id="ab965-136">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ab965-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ab965-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab965-137">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ab965-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ab965-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ab965-139">C#</span><span class="sxs-lookup"><span data-stu-id="ab965-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_bookingstaffmember_from_bookingbusiness-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ab965-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="ab965-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_bookingstaffmember_from_bookingbusiness-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ab965-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="ab965-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_bookingstaffmember_from_bookingbusiness-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-post-staffmembers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-post-staffmembers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-post-staffmembers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
