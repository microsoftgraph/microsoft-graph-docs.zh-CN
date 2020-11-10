---
title: 创建 bookingBusiness
description: 在租户中创建新的 Microsoft 预订业务。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 0dca36dd9c07eee0f3c91d0a5c25251672a400fa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960690"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="efd6e-103">创建 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="efd6e-103">Create bookingBusiness</span></span>

<span data-ttu-id="efd6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efd6e-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efd6e-105">在租户中创建新的 Microsoft 预订业务。</span><span class="sxs-lookup"><span data-stu-id="efd6e-105">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="efd6e-106">这是设置预订业务（必须在其中指定业务显示名称）的第一步。</span><span class="sxs-lookup"><span data-stu-id="efd6e-106">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="efd6e-107">您可以包含其他信息（如商务地址、网站地址和计划策略），也可以在以后通过 [更新](bookingbusiness-update.md) **bookingBusiness** 来设置该信息。</span><span class="sxs-lookup"><span data-stu-id="efd6e-107">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="efd6e-108">权限</span><span class="sxs-lookup"><span data-stu-id="efd6e-108">Permissions</span></span>
<span data-ttu-id="efd6e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efd6e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd6e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="efd6e-111">Permission type</span></span>      | <span data-ttu-id="efd6e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="efd6e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efd6e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efd6e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="efd6e-114">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="efd6e-114">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="efd6e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efd6e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efd6e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="efd6e-116">Not supported.</span></span>   |
|<span data-ttu-id="efd6e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="efd6e-117">Application</span></span> | <span data-ttu-id="efd6e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="efd6e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="efd6e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efd6e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="efd6e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="efd6e-120">Request headers</span></span>
| <span data-ttu-id="efd6e-121">名称</span><span class="sxs-lookup"><span data-stu-id="efd6e-121">Name</span></span>       | <span data-ttu-id="efd6e-122">说明</span><span class="sxs-lookup"><span data-stu-id="efd6e-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="efd6e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="efd6e-123">Authorization</span></span>  | <span data-ttu-id="efd6e-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="efd6e-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="efd6e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="efd6e-125">Request body</span></span>
<span data-ttu-id="efd6e-126">在请求正文中，提供 [bookingBusiness](../resources/bookingbusiness.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efd6e-126">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="efd6e-127">响应</span><span class="sxs-lookup"><span data-stu-id="efd6e-127">Response</span></span>
<span data-ttu-id="efd6e-128">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和 [bookingBusiness](../resources/bookingbusiness.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="efd6e-128">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efd6e-129">示例</span><span class="sxs-lookup"><span data-stu-id="efd6e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="efd6e-130">请求</span><span class="sxs-lookup"><span data-stu-id="efd6e-130">Request</span></span>
<span data-ttu-id="efd6e-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="efd6e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="efd6e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="efd6e-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="efd6e-133">C#</span><span class="sxs-lookup"><span data-stu-id="efd6e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingbusiness-from-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efd6e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efd6e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingbusiness-from-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efd6e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efd6e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingbusiness-from-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="efd6e-136">Java</span><span class="sxs-lookup"><span data-stu-id="efd6e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingbusiness-from-bookingbusinesses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="efd6e-137">在请求正文中，提供 [bookingBusiness](../resources/bookingbusiness.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efd6e-137">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="efd6e-138">响应</span><span class="sxs-lookup"><span data-stu-id="efd6e-138">Response</span></span>
<span data-ttu-id="efd6e-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="efd6e-139">The following is an example of the response.</span></span> <span data-ttu-id="efd6e-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="efd6e-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="efd6e-141">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efd6e-141">All of the properties will be returned from an actual call.</span></span>
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


