---
title: 创建 bookingBusiness
description: 在租户中创建新的 Microsoft 预订业务。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e3a41adb95f6749fcbdbdb83af8fbc2cba874ee2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636126"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="10e05-103">创建 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="10e05-103">Create bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10e05-104">在租户中创建新的 Microsoft 预订业务。</span><span class="sxs-lookup"><span data-stu-id="10e05-104">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="10e05-105">这是设置预订业务 (必须在其中指定业务显示名称) 的第一步。</span><span class="sxs-lookup"><span data-stu-id="10e05-105">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="10e05-106">您可以包含其他信息 (如商务地址、网站地址和计划策略), 也可以在以后通过[更新](bookingbusiness-update.md) **bookingBusiness**来设置该信息。</span><span class="sxs-lookup"><span data-stu-id="10e05-106">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="10e05-107">权限</span><span class="sxs-lookup"><span data-stu-id="10e05-107">Permissions</span></span>
<span data-ttu-id="10e05-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10e05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10e05-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="10e05-110">Permission type</span></span>      | <span data-ttu-id="10e05-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10e05-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10e05-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10e05-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="10e05-113">预订。全部</span><span class="sxs-lookup"><span data-stu-id="10e05-113">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="10e05-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10e05-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10e05-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="10e05-115">Not supported.</span></span>   |
|<span data-ttu-id="10e05-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="10e05-116">Application</span></span> | <span data-ttu-id="10e05-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="10e05-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10e05-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10e05-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="10e05-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="10e05-119">Request headers</span></span>
| <span data-ttu-id="10e05-120">名称</span><span class="sxs-lookup"><span data-stu-id="10e05-120">Name</span></span>       | <span data-ttu-id="10e05-121">说明</span><span class="sxs-lookup"><span data-stu-id="10e05-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="10e05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="10e05-122">Authorization</span></span>  | <span data-ttu-id="10e05-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="10e05-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="10e05-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="10e05-124">Request body</span></span>
<span data-ttu-id="10e05-125">在请求正文中, 提供[bookingBusiness](../resources/bookingbusiness.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10e05-125">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="10e05-126">响应</span><span class="sxs-lookup"><span data-stu-id="10e05-126">Response</span></span>
<span data-ttu-id="10e05-127">如果成功, 此方法在`201, Created`响应正文中返回响应代码和[bookingBusiness](../resources/bookingbusiness.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10e05-127">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10e05-128">示例</span><span class="sxs-lookup"><span data-stu-id="10e05-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10e05-129">请求</span><span class="sxs-lookup"><span data-stu-id="10e05-129">Request</span></span>
<span data-ttu-id="10e05-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="10e05-130">The following is an example of the request.</span></span>
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
<span data-ttu-id="10e05-131">在请求正文中, 提供[bookingBusiness](../resources/bookingbusiness.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10e05-131">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="10e05-132">响应</span><span class="sxs-lookup"><span data-stu-id="10e05-132">Response</span></span>
<span data-ttu-id="10e05-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="10e05-133">The following is an example of the response.</span></span> <span data-ttu-id="10e05-134">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="10e05-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="10e05-135">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10e05-135">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="10e05-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="10e05-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="10e05-137">语言</span><span class="sxs-lookup"><span data-stu-id="10e05-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_bookingbusiness_from_bookingbusinesses-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10e05-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="10e05-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_bookingbusiness_from_bookingbusinesses-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-bookingbusinesses.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-post-bookingbusinesses.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
