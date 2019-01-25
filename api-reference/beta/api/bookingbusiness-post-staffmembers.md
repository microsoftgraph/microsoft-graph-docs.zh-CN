---
title: 创建 bookingStaffMember
description: 在指定 bookingbusiness 中创建新的员工成员。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f3f13f30f646da8bf0fc8e32075002c0e591e902
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518609"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="638fb-103">创建 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="638fb-103">Create bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="638fb-104">在指定[bookingbusiness](../resources/bookingbusiness.md)中创建一个新[员工成员](../resources/bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="638fb-104">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="638fb-105">权限</span><span class="sxs-lookup"><span data-stu-id="638fb-105">Permissions</span></span>
<span data-ttu-id="638fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="638fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="638fb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="638fb-108">Permission type</span></span>      | <span data-ttu-id="638fb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="638fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="638fb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="638fb-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="638fb-111">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="638fb-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="638fb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="638fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="638fb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="638fb-113">Not supported.</span></span>   |
|<span data-ttu-id="638fb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="638fb-114">Application</span></span> | <span data-ttu-id="638fb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="638fb-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="638fb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="638fb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="638fb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="638fb-117">Request headers</span></span>
| <span data-ttu-id="638fb-118">名称</span><span class="sxs-lookup"><span data-stu-id="638fb-118">Name</span></span>       | <span data-ttu-id="638fb-119">说明</span><span class="sxs-lookup"><span data-stu-id="638fb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="638fb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="638fb-120">Authorization</span></span>  | <span data-ttu-id="638fb-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="638fb-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="638fb-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="638fb-122">Request body</span></span>
<span data-ttu-id="638fb-123">在请求正文中，提供[bookingStaffMember](../resources/bookingstaffmember.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="638fb-123">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="638fb-124">您必须包括以下属性：</span><span class="sxs-lookup"><span data-stu-id="638fb-124">You must include the following properties:</span></span>

- <span data-ttu-id="638fb-125">**displayName**</span><span class="sxs-lookup"><span data-stu-id="638fb-125">**displayName**</span></span>
- <span data-ttu-id="638fb-126">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="638fb-126">**emailAddress**</span></span>
- <span data-ttu-id="638fb-127">**角色**</span><span class="sxs-lookup"><span data-stu-id="638fb-127">**role**</span></span>


## <a name="response"></a><span data-ttu-id="638fb-128">响应</span><span class="sxs-lookup"><span data-stu-id="638fb-128">Response</span></span>
<span data-ttu-id="638fb-129">如果成功，此方法返回`201, Created`响应正文中的响应代码和[bookingStaffMember](../resources/bookingstaffmember.md)对象。</span><span class="sxs-lookup"><span data-stu-id="638fb-129">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="638fb-130">示例</span><span class="sxs-lookup"><span data-stu-id="638fb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="638fb-131">请求</span><span class="sxs-lookup"><span data-stu-id="638fb-131">Request</span></span>
<span data-ttu-id="638fb-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="638fb-132">The following is an example of the request.</span></span>
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
<span data-ttu-id="638fb-133">在请求正文中，提供[bookingStaffMember](../resources/bookingstaffmember.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="638fb-133">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="638fb-134">响应</span><span class="sxs-lookup"><span data-stu-id="638fb-134">Response</span></span>
<span data-ttu-id="638fb-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="638fb-135">The following is an example of the response.</span></span> <span data-ttu-id="638fb-136">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="638fb-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="638fb-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="638fb-137">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-post-staffmembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
