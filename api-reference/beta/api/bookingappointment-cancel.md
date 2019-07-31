---
title: 'bookingAppointment: 取消'
description: 在指定的 bookingbusiness 中取消指定的 bookingAppointment, 并向相关的 customer 和教职员工成员发送一封邮件。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d7be27f56ce9ab6aeed9feb539fbda1e297860d4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945282"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="05e16-103">bookingAppointment: 取消</span><span class="sxs-lookup"><span data-stu-id="05e16-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05e16-104">在指定的[bookingbusiness](../resources/bookingbusiness.md)中取消指定的[bookingAppointment](../resources/bookingappointment.md) , 并向相关的 customer 和教职员工成员发送一封邮件。</span><span class="sxs-lookup"><span data-stu-id="05e16-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="05e16-105">权限</span><span class="sxs-lookup"><span data-stu-id="05e16-105">Permissions</span></span>
<span data-ttu-id="05e16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05e16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05e16-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="05e16-108">Permission type</span></span>      | <span data-ttu-id="05e16-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05e16-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05e16-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05e16-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="05e16-111">BookingsAppointment, 全部, 全部登记, 全部, 预订。 All</span><span class="sxs-lookup"><span data-stu-id="05e16-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="05e16-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05e16-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05e16-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="05e16-113">Not supported.</span></span>   |
|<span data-ttu-id="05e16-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="05e16-114">Application</span></span> | <span data-ttu-id="05e16-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="05e16-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="05e16-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05e16-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="05e16-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="05e16-117">Request headers</span></span>
| <span data-ttu-id="05e16-118">名称</span><span class="sxs-lookup"><span data-stu-id="05e16-118">Name</span></span>       | <span data-ttu-id="05e16-119">说明</span><span class="sxs-lookup"><span data-stu-id="05e16-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="05e16-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="05e16-120">Authorization</span></span>  | <span data-ttu-id="05e16-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="05e16-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="05e16-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="05e16-122">Request body</span></span>
<span data-ttu-id="05e16-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="05e16-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="05e16-124">参数</span><span class="sxs-lookup"><span data-stu-id="05e16-124">Parameter</span></span>    | <span data-ttu-id="05e16-125">类型</span><span class="sxs-lookup"><span data-stu-id="05e16-125">Type</span></span>   |<span data-ttu-id="05e16-126">说明</span><span class="sxs-lookup"><span data-stu-id="05e16-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05e16-127">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="05e16-127">cancellationMessage</span></span>|<span data-ttu-id="05e16-128">String</span><span class="sxs-lookup"><span data-stu-id="05e16-128">String</span></span>|<span data-ttu-id="05e16-129">向客户确认约会已被取消的消息。</span><span class="sxs-lookup"><span data-stu-id="05e16-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="05e16-130">响应</span><span class="sxs-lookup"><span data-stu-id="05e16-130">Response</span></span>
<span data-ttu-id="05e16-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="05e16-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="05e16-133">如果您尝试取消不 exisit 的约会, 则此方法将返回`HTTP 404 Not found`。</span><span class="sxs-lookup"><span data-stu-id="05e16-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="05e16-134">示例</span><span class="sxs-lookup"><span data-stu-id="05e16-134">Example</span></span>
<span data-ttu-id="05e16-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="05e16-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="05e16-136">请求</span><span class="sxs-lookup"><span data-stu-id="05e16-136">Request</span></span>
<span data-ttu-id="05e16-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="05e16-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="05e16-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="05e16-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="05e16-139">C#</span><span class="sxs-lookup"><span data-stu-id="05e16-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05e16-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="05e16-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="05e16-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="05e16-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="05e16-142">Java</span><span class="sxs-lookup"><span data-stu-id="05e16-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingappointment-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="05e16-143">响应</span><span class="sxs-lookup"><span data-stu-id="05e16-143">Response</span></span>
<span data-ttu-id="05e16-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="05e16-144">The following is an example of the response.</span></span>
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
