---
title: 创建 bookingCustomer
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: ea534616c35f2ca43c7fb5b0b5169cc935aef1d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819451"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="0cf12-104">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="0cf12-104">Create bookingCustomer</span></span>

 > <span data-ttu-id="0cf12-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0cf12-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cf12-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0cf12-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="0cf12-107">创建新的[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0cf12-107">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0cf12-108">权限</span><span class="sxs-lookup"><span data-stu-id="0cf12-108">Permissions</span></span>
<span data-ttu-id="0cf12-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0cf12-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cf12-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cf12-111">Permission type</span></span>      | <span data-ttu-id="0cf12-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0cf12-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cf12-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cf12-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="0cf12-114">BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All，Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0cf12-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0cf12-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cf12-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cf12-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cf12-116">Not supported.</span></span>   |
|<span data-ttu-id="0cf12-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cf12-117">Application</span></span> | <span data-ttu-id="0cf12-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cf12-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="0cf12-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cf12-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="0cf12-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cf12-120">Request headers</span></span>
| <span data-ttu-id="0cf12-121">名称</span><span class="sxs-lookup"><span data-stu-id="0cf12-121">Name</span></span>       | <span data-ttu-id="0cf12-122">说明</span><span class="sxs-lookup"><span data-stu-id="0cf12-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0cf12-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cf12-123">Authorization</span></span>  | <span data-ttu-id="0cf12-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0cf12-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cf12-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cf12-125">Request body</span></span>
<span data-ttu-id="0cf12-126">在请求正文中，提供[bookingCustomer](../resources/bookingcustomer.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cf12-126">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="0cf12-127">响应</span><span class="sxs-lookup"><span data-stu-id="0cf12-127">Response</span></span>
<span data-ttu-id="0cf12-128">如果成功，此方法返回`201, Created`响应正文中的响应代码和[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0cf12-128">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cf12-129">示例</span><span class="sxs-lookup"><span data-stu-id="0cf12-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cf12-130">请求</span><span class="sxs-lookup"><span data-stu-id="0cf12-130">Request</span></span>
<span data-ttu-id="0cf12-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0cf12-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomer_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers

Content-type: application/json

{
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
<span data-ttu-id="0cf12-132">在请求正文中，提供[bookingCustomer](../resources/bookingcustomer.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cf12-132">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0cf12-133">响应</span><span class="sxs-lookup"><span data-stu-id="0cf12-133">Response</span></span>
<span data-ttu-id="0cf12-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0cf12-134">The following is an example of the response.</span></span> <span data-ttu-id="0cf12-135">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0cf12-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0cf12-136">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0cf12-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "36038f36-634e-44e4-9415-d7d59c2347aa",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
