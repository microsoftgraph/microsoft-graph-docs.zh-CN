---
title: bookingAppointment： 取消
description: 取消指定的 bookingAppointment 中指定的 bookingbusiness，并向所涉及的客户和人员成员发送消息。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c202ea309641bdcda3e1124792fdc04ad97e02ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514682"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="67483-103">bookingAppointment： 取消</span><span class="sxs-lookup"><span data-stu-id="67483-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67483-104">取消指定的[bookingAppointment](../resources/bookingappointment.md)中指定[bookingbusiness](../resources/bookingbusiness.md)，并向所涉及的客户和员工发送消息。</span><span class="sxs-lookup"><span data-stu-id="67483-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="67483-105">权限</span><span class="sxs-lookup"><span data-stu-id="67483-105">Permissions</span></span>
<span data-ttu-id="67483-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67483-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="67483-108">Permission type</span></span>      | <span data-ttu-id="67483-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67483-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67483-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67483-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="67483-111">BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All，Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="67483-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="67483-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67483-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67483-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="67483-113">Not supported.</span></span>   |
|<span data-ttu-id="67483-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="67483-114">Application</span></span> | <span data-ttu-id="67483-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="67483-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="67483-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67483-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="67483-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="67483-117">Request headers</span></span>
| <span data-ttu-id="67483-118">名称</span><span class="sxs-lookup"><span data-stu-id="67483-118">Name</span></span>       | <span data-ttu-id="67483-119">说明</span><span class="sxs-lookup"><span data-stu-id="67483-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="67483-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="67483-120">Authorization</span></span>  | <span data-ttu-id="67483-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="67483-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="67483-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="67483-122">Request body</span></span>
<span data-ttu-id="67483-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="67483-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="67483-124">参数</span><span class="sxs-lookup"><span data-stu-id="67483-124">Parameter</span></span>    | <span data-ttu-id="67483-125">类型</span><span class="sxs-lookup"><span data-stu-id="67483-125">Type</span></span>   |<span data-ttu-id="67483-126">说明</span><span class="sxs-lookup"><span data-stu-id="67483-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67483-127">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="67483-127">cancellationMessage</span></span>|<span data-ttu-id="67483-128">String</span><span class="sxs-lookup"><span data-stu-id="67483-128">String</span></span>|<span data-ttu-id="67483-129">要与客户约会已被取消的确认消息。</span><span class="sxs-lookup"><span data-stu-id="67483-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="67483-130">响应</span><span class="sxs-lookup"><span data-stu-id="67483-130">Response</span></span>
<span data-ttu-id="67483-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="67483-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="67483-133">如果您尝试取消约会不存在，则此方法返回`HTTP 404 Not found`。</span><span class="sxs-lookup"><span data-stu-id="67483-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="67483-134">示例</span><span class="sxs-lookup"><span data-stu-id="67483-134">Example</span></span>
<span data-ttu-id="67483-135">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="67483-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="67483-136">请求</span><span class="sxs-lookup"><span data-stu-id="67483-136">Request</span></span>
<span data-ttu-id="67483-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67483-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="67483-138">响应</span><span class="sxs-lookup"><span data-stu-id="67483-138">Response</span></span>
<span data-ttu-id="67483-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67483-139">The following is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/bookingappointment-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
