---
title: bookingBusiness： 取消发布
description: 对外部客户进行此业务计划页上不可用。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0b6c8122d37e5f6cdb1698b0d86295156e3481a0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517524"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="efd8e-103">bookingBusiness： 取消发布</span><span class="sxs-lookup"><span data-stu-id="efd8e-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efd8e-104">对外部客户进行此业务计划页上不可用。</span><span class="sxs-lookup"><span data-stu-id="efd8e-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="efd8e-105">**IsPublished**属性设置为 false，并**publicUrl**属性设为 null。</span><span class="sxs-lookup"><span data-stu-id="efd8e-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="efd8e-106">权限</span><span class="sxs-lookup"><span data-stu-id="efd8e-106">Permissions</span></span>
<span data-ttu-id="efd8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efd8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd8e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="efd8e-109">Permission type</span></span>      | <span data-ttu-id="efd8e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="efd8e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efd8e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efd8e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="efd8e-112">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="efd8e-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="efd8e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efd8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efd8e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="efd8e-114">Not supported.</span></span>   |
|<span data-ttu-id="efd8e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="efd8e-115">Application</span></span> | <span data-ttu-id="efd8e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="efd8e-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="efd8e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efd8e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="efd8e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="efd8e-118">Request headers</span></span>
| <span data-ttu-id="efd8e-119">名称</span><span class="sxs-lookup"><span data-stu-id="efd8e-119">Name</span></span>       | <span data-ttu-id="efd8e-120">说明</span><span class="sxs-lookup"><span data-stu-id="efd8e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="efd8e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="efd8e-121">Authorization</span></span>  | <span data-ttu-id="efd8e-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="efd8e-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="efd8e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="efd8e-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="efd8e-124">响应</span><span class="sxs-lookup"><span data-stu-id="efd8e-124">Response</span></span>
<span data-ttu-id="efd8e-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="efd8e-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efd8e-127">示例</span><span class="sxs-lookup"><span data-stu-id="efd8e-127">Example</span></span>
<span data-ttu-id="efd8e-128">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="efd8e-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="efd8e-129">请求</span><span class="sxs-lookup"><span data-stu-id="efd8e-129">Request</span></span>
<span data-ttu-id="efd8e-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="efd8e-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="efd8e-131">响应</span><span class="sxs-lookup"><span data-stu-id="efd8e-131">Response</span></span>
<span data-ttu-id="efd8e-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="efd8e-132">The following is an example of the response.</span></span>
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
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
