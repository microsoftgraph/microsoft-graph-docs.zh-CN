---
title: bookingBusiness： 发布
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 33e11fac5690e66664038705b482480ef689db6e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917319"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="a400e-104">bookingBusiness： 发布</span><span class="sxs-lookup"><span data-stu-id="a400e-104">bookingBusiness: publish</span></span>

 > <span data-ttu-id="a400e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a400e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a400e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a400e-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="a400e-107">将此业务的计划页提供给外部的客户。</span><span class="sxs-lookup"><span data-stu-id="a400e-107">Make the scheduling page of this business available to external customers.</span></span> 

<span data-ttu-id="a400e-108">**IsPublished**属性设置为 true，并**publicUrl**属性设为计划页的 URL。</span><span class="sxs-lookup"><span data-stu-id="a400e-108">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="a400e-109">权限</span><span class="sxs-lookup"><span data-stu-id="a400e-109">Permissions</span></span>
<span data-ttu-id="a400e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a400e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a400e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a400e-112">Permission type</span></span>      | <span data-ttu-id="a400e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a400e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a400e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a400e-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="a400e-115">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a400e-115">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a400e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a400e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a400e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a400e-117">Not supported.</span></span>   |
|<span data-ttu-id="a400e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a400e-118">Application</span></span> | <span data-ttu-id="a400e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a400e-119">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="a400e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a400e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="a400e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a400e-121">Request headers</span></span>
| <span data-ttu-id="a400e-122">名称</span><span class="sxs-lookup"><span data-stu-id="a400e-122">Name</span></span>       | <span data-ttu-id="a400e-123">说明</span><span class="sxs-lookup"><span data-stu-id="a400e-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a400e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a400e-124">Authorization</span></span>  | <span data-ttu-id="a400e-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a400e-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a400e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a400e-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a400e-127">响应</span><span class="sxs-lookup"><span data-stu-id="a400e-127">Response</span></span>
<span data-ttu-id="a400e-p104">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a400e-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a400e-130">示例</span><span class="sxs-lookup"><span data-stu-id="a400e-130">Example</span></span>
<span data-ttu-id="a400e-131">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a400e-131">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a400e-132">请求</span><span class="sxs-lookup"><span data-stu-id="a400e-132">Request</span></span>
<span data-ttu-id="a400e-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a400e-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="a400e-134">响应</span><span class="sxs-lookup"><span data-stu-id="a400e-134">Response</span></span>
<span data-ttu-id="a400e-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a400e-135">The following is an example of the response.</span></span> 
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
