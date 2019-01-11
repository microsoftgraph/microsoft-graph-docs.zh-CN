---
title: 创建 bookingBusiness
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: bfecb479a04f991799eb239c643e2cc521d8332c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894472"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="ced1d-104">创建 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="ced1d-104">Create bookingBusiness</span></span>

 > <span data-ttu-id="ced1d-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ced1d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ced1d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ced1d-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="ced1d-107">在租户中创建新的 Microsoft 预订业务。</span><span class="sxs-lookup"><span data-stu-id="ced1d-107">Create a new Microsoft Bookings business in a tenant.</span></span> 

<span data-ttu-id="ced1d-108">这是设置预订业务其中必须指定业务显示名称的第一步。</span><span class="sxs-lookup"><span data-stu-id="ced1d-108">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="ced1d-109">您可以包括其他信息，如业务地址、 网站地址和计划策略，或者该信息稍后通过设置[更新](bookingbusiness-update.md) **bookingBusiness**。</span><span class="sxs-lookup"><span data-stu-id="ced1d-109">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="ced1d-110">权限</span><span class="sxs-lookup"><span data-stu-id="ced1d-110">Permissions</span></span>
<span data-ttu-id="ced1d-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ced1d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ced1d-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="ced1d-113">Permission type</span></span>      | <span data-ttu-id="ced1d-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ced1d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ced1d-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ced1d-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="ced1d-116">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ced1d-116">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="ced1d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ced1d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ced1d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ced1d-118">Not supported.</span></span>   |
|<span data-ttu-id="ced1d-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="ced1d-119">Application</span></span> | <span data-ttu-id="ced1d-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ced1d-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ced1d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ced1d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="ced1d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ced1d-122">Request headers</span></span>
| <span data-ttu-id="ced1d-123">名称</span><span class="sxs-lookup"><span data-stu-id="ced1d-123">Name</span></span>       | <span data-ttu-id="ced1d-124">说明</span><span class="sxs-lookup"><span data-stu-id="ced1d-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ced1d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ced1d-125">Authorization</span></span>  | <span data-ttu-id="ced1d-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ced1d-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ced1d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ced1d-127">Request body</span></span>
<span data-ttu-id="ced1d-128">在请求正文中，提供[bookingBusiness](../resources/bookingbusiness.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ced1d-128">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ced1d-129">响应</span><span class="sxs-lookup"><span data-stu-id="ced1d-129">Response</span></span>
<span data-ttu-id="ced1d-130">如果成功，此方法返回`201, Created`响应正文中的响应代码和[bookingBusiness](../resources/bookingbusiness.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ced1d-130">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ced1d-131">示例</span><span class="sxs-lookup"><span data-stu-id="ced1d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ced1d-132">请求</span><span class="sxs-lookup"><span data-stu-id="ced1d-132">Request</span></span>
<span data-ttu-id="ced1d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ced1d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingbusiness_from_bookingbusinesses"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Content-type: application/json

{
    "displayName":"Fourth Coffee",
    "address":{
        "type":"mall",
        "postOfficeBox":"P.O. Box 123",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "phone":"206-555-0100",
    "email":"manager@fourthcoffee.com",
    "webSiteUrl":"https://www.fourthcoffee.com",
    "defaultCurrencyIso":"USD"
}
```
<span data-ttu-id="ced1d-134">在请求正文中，提供[bookingBusiness](../resources/bookingbusiness.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ced1d-134">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ced1d-135">响应</span><span class="sxs-lookup"><span data-stu-id="ced1d-135">Response</span></span>
<span data-ttu-id="ced1d-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ced1d-136">The following is an example of the response.</span></span> <span data-ttu-id="ced1d-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ced1d-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ced1d-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ced1d-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses/$entity",
    "id":"fourthcoffee@M365B489948.onmicrosoft.com",
    "displayName":"Fourth Coffee",
    "businessType":"",
    "phone":"206-555-0100",
    "email":"manager@fourthcoffee.com",
    "webSiteUrl":"https://www.fourthcoffee.com",
    "defaultCurrencyIso":"USD",
    "isPublished":false,
    "publicUrl":null,
    "address":{
        "type":"mall",
        "postOfficeBox":"P.O. Box 123",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "businessHours":[
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
    ],
    "schedulingPolicy":{
        "timeSlotInterval":"PT30M",
        "minimumLeadTime":"P1D",
        "maximumAdvance":"P365D",
        "sendConfirmationsToOwner":true,
        "allowStaffSelection":true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
