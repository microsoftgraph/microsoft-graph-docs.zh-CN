---
title: 删除 bookingAppointment
description: 删除指定 bookingbusiness 中的 bookingAppointment。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 41a5096809b91ee25dfe8dc70071aa37c08aebb5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047936"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="12c9a-103">删除 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="12c9a-103">Delete bookingAppointment</span></span>

<span data-ttu-id="12c9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12c9a-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12c9a-105">删除指定的 bookingbusiness 中的[bookingAppointment。](../resources/bookingbusiness.md) [](../resources/bookingappointment.md)</span><span class="sxs-lookup"><span data-stu-id="12c9a-105">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="12c9a-106">权限</span><span class="sxs-lookup"><span data-stu-id="12c9a-106">Permissions</span></span>
<span data-ttu-id="12c9a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12c9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12c9a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="12c9a-109">Permission type</span></span>      | <span data-ttu-id="12c9a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12c9a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12c9a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12c9a-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="12c9a-112">BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="12c9a-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="12c9a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12c9a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12c9a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="12c9a-114">Not supported.</span></span>   |
|<span data-ttu-id="12c9a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="12c9a-115">Application</span></span> | <span data-ttu-id="12c9a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12c9a-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="12c9a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12c9a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="12c9a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="12c9a-118">Request headers</span></span>
| <span data-ttu-id="12c9a-119">名称</span><span class="sxs-lookup"><span data-stu-id="12c9a-119">Name</span></span>       | <span data-ttu-id="12c9a-120">说明</span><span class="sxs-lookup"><span data-stu-id="12c9a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="12c9a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="12c9a-121">Authorization</span></span>  | <span data-ttu-id="12c9a-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="12c9a-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="12c9a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="12c9a-123">Request body</span></span>
<span data-ttu-id="12c9a-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="12c9a-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="12c9a-125">响应</span><span class="sxs-lookup"><span data-stu-id="12c9a-125">Response</span></span>
<span data-ttu-id="12c9a-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="12c9a-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12c9a-128">示例</span><span class="sxs-lookup"><span data-stu-id="12c9a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12c9a-129">请求</span><span class="sxs-lookup"><span data-stu-id="12c9a-129">Request</span></span>
<span data-ttu-id="12c9a-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="12c9a-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12c9a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="12c9a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
# <a name="c"></a>[<span data-ttu-id="12c9a-132">C#</span><span class="sxs-lookup"><span data-stu-id="12c9a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12c9a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12c9a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12c9a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12c9a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12c9a-135">Java</span><span class="sxs-lookup"><span data-stu-id="12c9a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="12c9a-136">响应</span><span class="sxs-lookup"><span data-stu-id="12c9a-136">Response</span></span>
<span data-ttu-id="12c9a-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="12c9a-137">The following is an example of the response.</span></span> <span data-ttu-id="12c9a-138">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="12c9a-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


