---
title: 创建 bookingBusiness
description: 在租户中创建新的 Microsoft Bookings 业务。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 251d1b6d5e73b646216bdb152289808e93882d38
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047880"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="58f39-103">创建 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="58f39-103">Create bookingBusiness</span></span>

<span data-ttu-id="58f39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58f39-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58f39-105">在租户中创建新的 Microsoft Bookings 业务。</span><span class="sxs-lookup"><span data-stu-id="58f39-105">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="58f39-106">这是设置 Bookings 业务的第一步，你必须指定业务显示名称。</span><span class="sxs-lookup"><span data-stu-id="58f39-106">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="58f39-107">可以包括其他信息（如公司地址、网站地址和日程安排策略）或稍后通过更新 **bookingBusiness** 来 [](bookingbusiness-update.md)设置该信息。</span><span class="sxs-lookup"><span data-stu-id="58f39-107">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="58f39-108">权限</span><span class="sxs-lookup"><span data-stu-id="58f39-108">Permissions</span></span>
<span data-ttu-id="58f39-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58f39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58f39-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="58f39-111">Permission type</span></span>      | <span data-ttu-id="58f39-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58f39-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58f39-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58f39-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="58f39-114">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="58f39-114">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="58f39-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58f39-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58f39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="58f39-116">Not supported.</span></span>   |
|<span data-ttu-id="58f39-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="58f39-117">Application</span></span> | <span data-ttu-id="58f39-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="58f39-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58f39-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58f39-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="58f39-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="58f39-120">Request headers</span></span>
| <span data-ttu-id="58f39-121">名称</span><span class="sxs-lookup"><span data-stu-id="58f39-121">Name</span></span>       | <span data-ttu-id="58f39-122">说明</span><span class="sxs-lookup"><span data-stu-id="58f39-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="58f39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58f39-123">Authorization</span></span>  | <span data-ttu-id="58f39-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="58f39-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="58f39-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="58f39-125">Request body</span></span>
<span data-ttu-id="58f39-126">在请求正文中，提供 [bookingBusiness](../resources/bookingbusiness.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58f39-126">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="58f39-127">响应</span><span class="sxs-lookup"><span data-stu-id="58f39-127">Response</span></span>
<span data-ttu-id="58f39-128">如果成功，此方法在 `201, Created` 响应正文中返回 响应代码和 [bookingBusiness](../resources/bookingbusiness.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58f39-128">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58f39-129">示例</span><span class="sxs-lookup"><span data-stu-id="58f39-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58f39-130">请求</span><span class="sxs-lookup"><span data-stu-id="58f39-130">Request</span></span>
<span data-ttu-id="58f39-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="58f39-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58f39-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="58f39-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="58f39-133">C#</span><span class="sxs-lookup"><span data-stu-id="58f39-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingbusiness-from-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58f39-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58f39-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingbusiness-from-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58f39-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58f39-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingbusiness-from-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58f39-136">Java</span><span class="sxs-lookup"><span data-stu-id="58f39-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingbusiness-from-bookingbusinesses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="58f39-137">在请求正文中，提供 [bookingBusiness](../resources/bookingbusiness.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58f39-137">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="58f39-138">响应</span><span class="sxs-lookup"><span data-stu-id="58f39-138">Response</span></span>
<span data-ttu-id="58f39-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="58f39-139">The following is an example of the response.</span></span> <span data-ttu-id="58f39-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="58f39-140">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


