---
title: 'bookingAppointment: 取消'
description: 在指定的 bookingbusiness 中取消指定的 bookingAppointment, 并向相关的 customer 和教职员工成员发送一封邮件。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f80f97f6e085980d26ce4555f35f769db6a4f4e9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322549"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="ace01-103">bookingAppointment: 取消</span><span class="sxs-lookup"><span data-stu-id="ace01-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ace01-104">在指定的[bookingbusiness](../resources/bookingbusiness.md)中取消指定的[bookingAppointment](../resources/bookingappointment.md) , 并向相关的 customer 和教职员工成员发送一封邮件。</span><span class="sxs-lookup"><span data-stu-id="ace01-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="ace01-105">权限</span><span class="sxs-lookup"><span data-stu-id="ace01-105">Permissions</span></span>
<span data-ttu-id="ace01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ace01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ace01-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ace01-108">Permission type</span></span>      | <span data-ttu-id="ace01-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ace01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ace01-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ace01-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ace01-111">BookingsAppointment, 全部, 全部登记, 全部, 预订。 all</span><span class="sxs-lookup"><span data-stu-id="ace01-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ace01-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ace01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ace01-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ace01-113">Not supported.</span></span>   |
|<span data-ttu-id="ace01-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ace01-114">Application</span></span> | <span data-ttu-id="ace01-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ace01-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ace01-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ace01-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="ace01-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ace01-117">Request headers</span></span>
| <span data-ttu-id="ace01-118">名称</span><span class="sxs-lookup"><span data-stu-id="ace01-118">Name</span></span>       | <span data-ttu-id="ace01-119">说明</span><span class="sxs-lookup"><span data-stu-id="ace01-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ace01-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ace01-120">Authorization</span></span>  | <span data-ttu-id="ace01-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ace01-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ace01-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="ace01-122">Request body</span></span>
<span data-ttu-id="ace01-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ace01-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ace01-124">参数</span><span class="sxs-lookup"><span data-stu-id="ace01-124">Parameter</span></span>    | <span data-ttu-id="ace01-125">类型</span><span class="sxs-lookup"><span data-stu-id="ace01-125">Type</span></span>   |<span data-ttu-id="ace01-126">说明</span><span class="sxs-lookup"><span data-stu-id="ace01-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ace01-127">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="ace01-127">cancellationMessage</span></span>|<span data-ttu-id="ace01-128">String</span><span class="sxs-lookup"><span data-stu-id="ace01-128">String</span></span>|<span data-ttu-id="ace01-129">向客户确认约会已被取消的消息。</span><span class="sxs-lookup"><span data-stu-id="ace01-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="ace01-130">响应</span><span class="sxs-lookup"><span data-stu-id="ace01-130">Response</span></span>
<span data-ttu-id="ace01-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ace01-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="ace01-133">如果您尝试取消不 exisit 的约会, 则此方法将返回`HTTP 404 Not found`。</span><span class="sxs-lookup"><span data-stu-id="ace01-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="ace01-134">示例</span><span class="sxs-lookup"><span data-stu-id="ace01-134">Example</span></span>
<span data-ttu-id="ace01-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ace01-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ace01-136">请求</span><span class="sxs-lookup"><span data-stu-id="ace01-136">Request</span></span>
<span data-ttu-id="ace01-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ace01-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ace01-138">响应</span><span class="sxs-lookup"><span data-stu-id="ace01-138">Response</span></span>
<span data-ttu-id="ace01-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ace01-139">The following is an example of the response.</span></span>
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
  "suppressions": []
}
-->
