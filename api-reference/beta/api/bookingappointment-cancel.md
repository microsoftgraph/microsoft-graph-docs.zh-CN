---
title: bookingAppointment： 取消
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 2ea1baae613188037ab806a81a6341daecaddc65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917249"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="99939-104">bookingAppointment： 取消</span><span class="sxs-lookup"><span data-stu-id="99939-104">bookingAppointment: cancel</span></span>

 > <span data-ttu-id="99939-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="99939-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99939-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="99939-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="99939-107">取消指定的[bookingAppointment](../resources/bookingappointment.md)中指定[bookingbusiness](../resources/bookingbusiness.md)，并向所涉及的客户和员工发送消息。</span><span class="sxs-lookup"><span data-stu-id="99939-107">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="99939-108">权限</span><span class="sxs-lookup"><span data-stu-id="99939-108">Permissions</span></span>
<span data-ttu-id="99939-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99939-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99939-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="99939-111">Permission type</span></span>      | <span data-ttu-id="99939-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99939-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99939-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99939-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="99939-114">BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All，Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="99939-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="99939-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99939-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99939-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="99939-116">Not supported.</span></span>   |
|<span data-ttu-id="99939-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="99939-117">Application</span></span> | <span data-ttu-id="99939-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="99939-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="99939-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99939-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="99939-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="99939-120">Request headers</span></span>
| <span data-ttu-id="99939-121">名称</span><span class="sxs-lookup"><span data-stu-id="99939-121">Name</span></span>       | <span data-ttu-id="99939-122">说明</span><span class="sxs-lookup"><span data-stu-id="99939-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="99939-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99939-123">Authorization</span></span>  | <span data-ttu-id="99939-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="99939-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="99939-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="99939-125">Request body</span></span>
<span data-ttu-id="99939-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="99939-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="99939-127">参数</span><span class="sxs-lookup"><span data-stu-id="99939-127">Parameter</span></span>    | <span data-ttu-id="99939-128">类型</span><span class="sxs-lookup"><span data-stu-id="99939-128">Type</span></span>   |<span data-ttu-id="99939-129">说明</span><span class="sxs-lookup"><span data-stu-id="99939-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99939-130">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="99939-130">cancellationMessage</span></span>|<span data-ttu-id="99939-131">字符串</span><span class="sxs-lookup"><span data-stu-id="99939-131">String</span></span>|<span data-ttu-id="99939-132">要与客户约会已被取消的确认消息。</span><span class="sxs-lookup"><span data-stu-id="99939-132">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="99939-133">响应</span><span class="sxs-lookup"><span data-stu-id="99939-133">Response</span></span>
<span data-ttu-id="99939-p104">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="99939-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="99939-136">如果您尝试取消约会不存在，则此方法返回`HTTP 404 Not found`。</span><span class="sxs-lookup"><span data-stu-id="99939-136">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="99939-137">示例</span><span class="sxs-lookup"><span data-stu-id="99939-137">Example</span></span>
<span data-ttu-id="99939-138">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="99939-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99939-139">请求</span><span class="sxs-lookup"><span data-stu-id="99939-139">Request</span></span>
<span data-ttu-id="99939-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99939-140">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="99939-141">响应</span><span class="sxs-lookup"><span data-stu-id="99939-141">Response</span></span>
<span data-ttu-id="99939-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="99939-142">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
