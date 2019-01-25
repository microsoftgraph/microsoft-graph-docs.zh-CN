---
title: bookingBusiness： 发布
description: 将此业务的计划页提供给外部的客户。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 11d8bea864772c0bcc4365c056973fac782add5d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508655"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="1d787-103">bookingBusiness： 发布</span><span class="sxs-lookup"><span data-stu-id="1d787-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d787-104">将此业务的计划页提供给外部的客户。</span><span class="sxs-lookup"><span data-stu-id="1d787-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="1d787-105">**IsPublished**属性设置为 true，并**publicUrl**属性设为计划页的 URL。</span><span class="sxs-lookup"><span data-stu-id="1d787-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d787-106">权限</span><span class="sxs-lookup"><span data-stu-id="1d787-106">Permissions</span></span>
<span data-ttu-id="1d787-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d787-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d787-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d787-109">Permission type</span></span>      | <span data-ttu-id="1d787-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d787-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d787-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d787-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="1d787-112">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="1d787-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1d787-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d787-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d787-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d787-114">Not supported.</span></span>   |
|<span data-ttu-id="1d787-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d787-115">Application</span></span> | <span data-ttu-id="1d787-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d787-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1d787-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d787-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="1d787-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d787-118">Request headers</span></span>
| <span data-ttu-id="1d787-119">名称</span><span class="sxs-lookup"><span data-stu-id="1d787-119">Name</span></span>       | <span data-ttu-id="1d787-120">说明</span><span class="sxs-lookup"><span data-stu-id="1d787-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1d787-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d787-121">Authorization</span></span>  | <span data-ttu-id="1d787-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1d787-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d787-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d787-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1d787-124">响应</span><span class="sxs-lookup"><span data-stu-id="1d787-124">Response</span></span>
<span data-ttu-id="1d787-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1d787-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d787-127">示例</span><span class="sxs-lookup"><span data-stu-id="1d787-127">Example</span></span>
<span data-ttu-id="1d787-128">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1d787-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1d787-129">请求</span><span class="sxs-lookup"><span data-stu-id="1d787-129">Request</span></span>
<span data-ttu-id="1d787-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1d787-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="1d787-131">响应</span><span class="sxs-lookup"><span data-stu-id="1d787-131">Response</span></span>
<span data-ttu-id="1d787-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1d787-132">The following is an example of the response.</span></span>
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
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
