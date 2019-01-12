---
title: 创建 bookingStaffMember
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: d9f1abd453601087daa524d550a6041c7960e634
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926503"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="d966e-104">创建 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="d966e-104">Create bookingStaffMember</span></span>

 > <span data-ttu-id="d966e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d966e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d966e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d966e-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="d966e-107">在指定[bookingbusiness](../resources/bookingbusiness.md)中创建一个新[员工成员](../resources/bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="d966e-107">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d966e-108">权限</span><span class="sxs-lookup"><span data-stu-id="d966e-108">Permissions</span></span>
<span data-ttu-id="d966e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d966e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d966e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d966e-111">Permission type</span></span>      | <span data-ttu-id="d966e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d966e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d966e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d966e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="d966e-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="d966e-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d966e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d966e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d966e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d966e-116">Not supported.</span></span>   |
|<span data-ttu-id="d966e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d966e-117">Application</span></span> | <span data-ttu-id="d966e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d966e-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d966e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d966e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="d966e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d966e-120">Request headers</span></span>
| <span data-ttu-id="d966e-121">名称</span><span class="sxs-lookup"><span data-stu-id="d966e-121">Name</span></span>       | <span data-ttu-id="d966e-122">说明</span><span class="sxs-lookup"><span data-stu-id="d966e-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d966e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d966e-123">Authorization</span></span>  | <span data-ttu-id="d966e-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d966e-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d966e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d966e-125">Request body</span></span>
<span data-ttu-id="d966e-126">在请求正文中，提供[bookingStaffMember](../resources/bookingstaffmember.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d966e-126">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="d966e-127">您必须包括以下属性：</span><span class="sxs-lookup"><span data-stu-id="d966e-127">You must include the following properties:</span></span>

- <span data-ttu-id="d966e-128">**displayName**</span><span class="sxs-lookup"><span data-stu-id="d966e-128">**displayName**</span></span>
- <span data-ttu-id="d966e-129">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="d966e-129">**emailAddress**</span></span>
- <span data-ttu-id="d966e-130">**角色**</span><span class="sxs-lookup"><span data-stu-id="d966e-130">**role**</span></span>


## <a name="response"></a><span data-ttu-id="d966e-131">响应</span><span class="sxs-lookup"><span data-stu-id="d966e-131">Response</span></span>
<span data-ttu-id="d966e-132">如果成功，此方法返回`201, Created`响应正文中的响应代码和[bookingStaffMember](../resources/bookingstaffmember.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d966e-132">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d966e-133">示例</span><span class="sxs-lookup"><span data-stu-id="d966e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d966e-134">请求</span><span class="sxs-lookup"><span data-stu-id="d966e-134">Request</span></span>
<span data-ttu-id="d966e-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d966e-135">The following is an example of the request.</span></span>
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
<span data-ttu-id="d966e-136">在请求正文中，提供[bookingStaffMember](../resources/bookingstaffmember.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d966e-136">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d966e-137">响应</span><span class="sxs-lookup"><span data-stu-id="d966e-137">Response</span></span>
<span data-ttu-id="d966e-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d966e-138">The following is an example of the response.</span></span> <span data-ttu-id="d966e-139">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d966e-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d966e-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d966e-140">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
