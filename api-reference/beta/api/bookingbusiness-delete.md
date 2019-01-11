---
title: 删除 bookingBusiness
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 273c3f3578653e457122b2bf045eb54644ea6b08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849915"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="8eaf1-104">删除 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="8eaf1-104">Delete bookingBusiness</span></span>

 > <span data-ttu-id="8eaf1-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8eaf1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eaf1-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8eaf1-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="8eaf1-107">删除[bookingBusiness](../resources/bookingbusiness.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8eaf1-107">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8eaf1-108">权限</span><span class="sxs-lookup"><span data-stu-id="8eaf1-108">Permissions</span></span>
<span data-ttu-id="8eaf1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8eaf1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eaf1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8eaf1-111">Permission type</span></span>      | <span data-ttu-id="8eaf1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8eaf1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8eaf1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8eaf1-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="8eaf1-114">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="8eaf1-114">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8eaf1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8eaf1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eaf1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8eaf1-116">Not supported.</span></span>   |
|<span data-ttu-id="8eaf1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8eaf1-117">Application</span></span> | <span data-ttu-id="8eaf1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8eaf1-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="8eaf1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8eaf1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="8eaf1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8eaf1-120">Request headers</span></span>
| <span data-ttu-id="8eaf1-121">名称</span><span class="sxs-lookup"><span data-stu-id="8eaf1-121">Name</span></span>       | <span data-ttu-id="8eaf1-122">说明</span><span class="sxs-lookup"><span data-stu-id="8eaf1-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8eaf1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eaf1-123">Authorization</span></span>  | <span data-ttu-id="8eaf1-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8eaf1-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eaf1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8eaf1-125">Request body</span></span>
<span data-ttu-id="8eaf1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8eaf1-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8eaf1-127">响应</span><span class="sxs-lookup"><span data-stu-id="8eaf1-127">Response</span></span>
<span data-ttu-id="8eaf1-p104">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8eaf1-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eaf1-130">示例</span><span class="sxs-lookup"><span data-stu-id="8eaf1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8eaf1-131">请求</span><span class="sxs-lookup"><span data-stu-id="8eaf1-131">Request</span></span>
<span data-ttu-id="8eaf1-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8eaf1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="8eaf1-133">响应</span><span class="sxs-lookup"><span data-stu-id="8eaf1-133">Response</span></span>
<span data-ttu-id="8eaf1-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8eaf1-134">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
