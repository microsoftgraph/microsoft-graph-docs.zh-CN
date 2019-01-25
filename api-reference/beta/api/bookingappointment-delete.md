---
title: 删除 bookingAppointment
description: 删除在指定 bookingbusiness bookingAppointment。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a8abe1961be7e3caf36c9d690497347f42c83fde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513716"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="a6356-103">删除 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="a6356-103">Delete bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6356-104">删除在指定[bookingbusiness](../resources/bookingbusiness.md) [bookingAppointment](../resources/bookingappointment.md) 。</span><span class="sxs-lookup"><span data-stu-id="a6356-104">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a6356-105">权限</span><span class="sxs-lookup"><span data-stu-id="a6356-105">Permissions</span></span>
<span data-ttu-id="a6356-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6356-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6356-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6356-108">Permission type</span></span>      | <span data-ttu-id="a6356-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6356-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6356-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6356-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a6356-111">BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All，Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a6356-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a6356-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6356-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6356-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6356-113">Not supported.</span></span>   |
|<span data-ttu-id="a6356-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6356-114">Application</span></span> | <span data-ttu-id="a6356-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6356-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a6356-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6356-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a6356-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6356-117">Request headers</span></span>
| <span data-ttu-id="a6356-118">名称</span><span class="sxs-lookup"><span data-stu-id="a6356-118">Name</span></span>       | <span data-ttu-id="a6356-119">说明</span><span class="sxs-lookup"><span data-stu-id="a6356-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a6356-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6356-120">Authorization</span></span>  | <span data-ttu-id="a6356-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a6356-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6356-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6356-122">Request body</span></span>
<span data-ttu-id="a6356-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6356-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a6356-124">响应</span><span class="sxs-lookup"><span data-stu-id="a6356-124">Response</span></span>
<span data-ttu-id="a6356-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a6356-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6356-127">示例</span><span class="sxs-lookup"><span data-stu-id="a6356-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6356-128">请求</span><span class="sxs-lookup"><span data-stu-id="a6356-128">Request</span></span>
<span data-ttu-id="a6356-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a6356-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
##### <a name="response"></a><span data-ttu-id="a6356-130">响应</span><span class="sxs-lookup"><span data-stu-id="a6356-130">Response</span></span>
<span data-ttu-id="a6356-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a6356-131">The following is an example of the response.</span></span> <span data-ttu-id="a6356-132">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a6356-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a6356-133">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6356-133">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingappointment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
