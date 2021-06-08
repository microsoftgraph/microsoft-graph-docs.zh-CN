---
title: bookingAppointment： cancel
description: 取消指定 bookingbusiness 中的指定 bookingAppointment，并将消息发送给涉及的客户和员工成员。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 4d05157faf95beaf6dab95742314472586f00063
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786269"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="4e869-103">bookingAppointment： cancel</span><span class="sxs-lookup"><span data-stu-id="4e869-103">bookingAppointment: cancel</span></span>

<span data-ttu-id="4e869-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e869-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e869-105">取消指定 bookingbusiness 中的指定[bookingAppointment，](../resources/bookingbusiness.md)并将消息发送给涉及的客户和员工成员。 [](../resources/bookingappointment.md)</span><span class="sxs-lookup"><span data-stu-id="4e869-105">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e869-106">权限</span><span class="sxs-lookup"><span data-stu-id="4e869-106">Permissions</span></span>
<span data-ttu-id="4e869-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e869-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e869-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e869-109">Permission type</span></span>      | <span data-ttu-id="4e869-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e869-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e869-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e869-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4e869-112">BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="4e869-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4e869-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e869-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e869-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e869-114">Not supported.</span></span>   |
|<span data-ttu-id="4e869-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e869-115">Application</span></span> | <span data-ttu-id="4e869-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e869-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4e869-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e869-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="4e869-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e869-118">Request headers</span></span>
| <span data-ttu-id="4e869-119">名称</span><span class="sxs-lookup"><span data-stu-id="4e869-119">Name</span></span>       | <span data-ttu-id="4e869-120">说明</span><span class="sxs-lookup"><span data-stu-id="4e869-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4e869-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e869-121">Authorization</span></span>  | <span data-ttu-id="4e869-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4e869-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e869-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e869-123">Request body</span></span>
<span data-ttu-id="4e869-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4e869-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4e869-125">参数</span><span class="sxs-lookup"><span data-stu-id="4e869-125">Parameter</span></span>    | <span data-ttu-id="4e869-126">类型</span><span class="sxs-lookup"><span data-stu-id="4e869-126">Type</span></span>   |<span data-ttu-id="4e869-127">说明</span><span class="sxs-lookup"><span data-stu-id="4e869-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e869-128">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="4e869-128">cancellationMessage</span></span>|<span data-ttu-id="4e869-129">String</span><span class="sxs-lookup"><span data-stu-id="4e869-129">String</span></span>|<span data-ttu-id="4e869-130">向客户确认约会已取消的消息。</span><span class="sxs-lookup"><span data-stu-id="4e869-130">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="4e869-131">响应</span><span class="sxs-lookup"><span data-stu-id="4e869-131">Response</span></span>
<span data-ttu-id="4e869-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4e869-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="4e869-134">如果您尝试取消未取消的约会，此方法将返回 `HTTP 404 Not found` 。</span><span class="sxs-lookup"><span data-stu-id="4e869-134">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="4e869-135">示例</span><span class="sxs-lookup"><span data-stu-id="4e869-135">Example</span></span>
<span data-ttu-id="4e869-136">下面是如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4e869-136">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4e869-137">请求</span><span class="sxs-lookup"><span data-stu-id="4e869-137">Request</span></span>
<span data-ttu-id="4e869-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4e869-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e869-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e869-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4e869-140">C#</span><span class="sxs-lookup"><span data-stu-id="4e869-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e869-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e869-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e869-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e869-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e869-143">Java</span><span class="sxs-lookup"><span data-stu-id="4e869-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingappointment-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4e869-144">响应</span><span class="sxs-lookup"><span data-stu-id="4e869-144">Response</span></span>
<span data-ttu-id="4e869-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4e869-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


