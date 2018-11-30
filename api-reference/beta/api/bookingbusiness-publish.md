---
title: bookingBusiness： 发布
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: b3145409de1371a164d86ad1cc52ea199d245f50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043347"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="b034b-104">bookingBusiness： 发布</span><span class="sxs-lookup"><span data-stu-id="b034b-104">bookingBusiness: publish</span></span>

 > <span data-ttu-id="b034b-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b034b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b034b-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b034b-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="b034b-107">将此业务的计划页提供给外部的客户。</span><span class="sxs-lookup"><span data-stu-id="b034b-107">Make the scheduling page of this business available to external customers.</span></span> 

<span data-ttu-id="b034b-108">**IsPublished**属性设置为 true，并**publicUrl**属性设为计划页的 URL。</span><span class="sxs-lookup"><span data-stu-id="b034b-108">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="b034b-109">权限</span><span class="sxs-lookup"><span data-stu-id="b034b-109">Permissions</span></span>
<span data-ttu-id="b034b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b034b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b034b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b034b-112">Permission type</span></span>      | <span data-ttu-id="b034b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b034b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b034b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b034b-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="b034b-115">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b034b-115">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b034b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b034b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b034b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b034b-117">Not supported.</span></span>   |
|<span data-ttu-id="b034b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b034b-118">Application</span></span> | <span data-ttu-id="b034b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b034b-119">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="b034b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b034b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="b034b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b034b-121">Request headers</span></span>
| <span data-ttu-id="b034b-122">名称</span><span class="sxs-lookup"><span data-stu-id="b034b-122">Name</span></span>       | <span data-ttu-id="b034b-123">说明</span><span class="sxs-lookup"><span data-stu-id="b034b-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b034b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b034b-124">Authorization</span></span>  | <span data-ttu-id="b034b-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b034b-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b034b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b034b-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b034b-127">响应</span><span class="sxs-lookup"><span data-stu-id="b034b-127">Response</span></span>
<span data-ttu-id="b034b-p104">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b034b-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b034b-130">示例</span><span class="sxs-lookup"><span data-stu-id="b034b-130">Example</span></span>
<span data-ttu-id="b034b-131">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b034b-131">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b034b-132">请求</span><span class="sxs-lookup"><span data-stu-id="b034b-132">Request</span></span>
<span data-ttu-id="b034b-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b034b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="b034b-134">响应</span><span class="sxs-lookup"><span data-stu-id="b034b-134">Response</span></span>
<span data-ttu-id="b034b-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b034b-135">The following is an example of the response.</span></span> 
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
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->