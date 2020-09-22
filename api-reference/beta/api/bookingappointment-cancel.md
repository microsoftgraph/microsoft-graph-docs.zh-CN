---
title: bookingAppointment：取消
description: 在指定的 bookingbusiness 中取消指定的 bookingAppointment，并向相关的 customer 和教职员工成员发送一封邮件。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 42a12bfd05dddf6306f6de22b07b2029d2f39e2d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988133"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="ae8ff-103">bookingAppointment：取消</span><span class="sxs-lookup"><span data-stu-id="ae8ff-103">bookingAppointment: cancel</span></span>

<span data-ttu-id="ae8ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae8ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae8ff-105">在指定的[bookingbusiness](../resources/bookingbusiness.md)中取消指定的[bookingAppointment](../resources/bookingappointment.md) ，并向相关的 customer 和教职员工成员发送一封邮件。</span><span class="sxs-lookup"><span data-stu-id="ae8ff-105">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae8ff-106">权限</span><span class="sxs-lookup"><span data-stu-id="ae8ff-106">Permissions</span></span>
<span data-ttu-id="ae8ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae8ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae8ff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae8ff-109">Permission type</span></span>      | <span data-ttu-id="ae8ff-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae8ff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae8ff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae8ff-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="ae8ff-112">BookingsAppointment，全部，全部登记，全部，预订。 All</span><span class="sxs-lookup"><span data-stu-id="ae8ff-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ae8ff-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae8ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae8ff-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae8ff-114">Not supported.</span></span>   |
|<span data-ttu-id="ae8ff-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae8ff-115">Application</span></span> | <span data-ttu-id="ae8ff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae8ff-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ae8ff-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae8ff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="ae8ff-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae8ff-118">Request headers</span></span>
| <span data-ttu-id="ae8ff-119">名称</span><span class="sxs-lookup"><span data-stu-id="ae8ff-119">Name</span></span>       | <span data-ttu-id="ae8ff-120">说明</span><span class="sxs-lookup"><span data-stu-id="ae8ff-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ae8ff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae8ff-121">Authorization</span></span>  | <span data-ttu-id="ae8ff-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ae8ff-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae8ff-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae8ff-123">Request body</span></span>
<span data-ttu-id="ae8ff-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ae8ff-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ae8ff-125">参数</span><span class="sxs-lookup"><span data-stu-id="ae8ff-125">Parameter</span></span>    | <span data-ttu-id="ae8ff-126">类型</span><span class="sxs-lookup"><span data-stu-id="ae8ff-126">Type</span></span>   |<span data-ttu-id="ae8ff-127">说明</span><span class="sxs-lookup"><span data-stu-id="ae8ff-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae8ff-128">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="ae8ff-128">cancellationMessage</span></span>|<span data-ttu-id="ae8ff-129">String</span><span class="sxs-lookup"><span data-stu-id="ae8ff-129">String</span></span>|<span data-ttu-id="ae8ff-130">向客户确认约会已被取消的消息。</span><span class="sxs-lookup"><span data-stu-id="ae8ff-130">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="ae8ff-131">响应</span><span class="sxs-lookup"><span data-stu-id="ae8ff-131">Response</span></span>
<span data-ttu-id="ae8ff-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ae8ff-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="ae8ff-134">如果您尝试取消不 exisit 的约会，则此方法将返回 `HTTP 404 Not found` 。</span><span class="sxs-lookup"><span data-stu-id="ae8ff-134">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="ae8ff-135">示例</span><span class="sxs-lookup"><span data-stu-id="ae8ff-135">Example</span></span>
<span data-ttu-id="ae8ff-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ae8ff-136">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae8ff-137">请求</span><span class="sxs-lookup"><span data-stu-id="ae8ff-137">Request</span></span>
<span data-ttu-id="ae8ff-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ae8ff-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae8ff-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae8ff-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingappointment_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel
Content-type: application/json

{
  "cancellationMessage": "Your appointment has been successfully cancelled. Please call us again."
}
```
# <a name="c"></a>[<span data-ttu-id="ae8ff-140">C#</span><span class="sxs-lookup"><span data-stu-id="ae8ff-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae8ff-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae8ff-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae8ff-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae8ff-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ae8ff-143">响应</span><span class="sxs-lookup"><span data-stu-id="ae8ff-143">Response</span></span>
<span data-ttu-id="ae8ff-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ae8ff-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


