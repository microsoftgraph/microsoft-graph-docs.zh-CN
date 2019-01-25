---
title: 删除 bookingBusiness
description: 删除 bookingBusiness 对象。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 88f07b46231a942098a157f00097393d60253982
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511896"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="8fd1a-103">删除 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="8fd1a-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fd1a-104">删除[bookingBusiness](../resources/bookingbusiness.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8fd1a-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8fd1a-105">权限</span><span class="sxs-lookup"><span data-stu-id="8fd1a-105">Permissions</span></span>
<span data-ttu-id="8fd1a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8fd1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fd1a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8fd1a-108">Permission type</span></span>      | <span data-ttu-id="8fd1a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8fd1a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fd1a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8fd1a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8fd1a-111">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="8fd1a-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8fd1a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8fd1a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fd1a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fd1a-113">Not supported.</span></span>   |
|<span data-ttu-id="8fd1a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8fd1a-114">Application</span></span> | <span data-ttu-id="8fd1a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fd1a-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8fd1a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8fd1a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="8fd1a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8fd1a-117">Request headers</span></span>
| <span data-ttu-id="8fd1a-118">名称</span><span class="sxs-lookup"><span data-stu-id="8fd1a-118">Name</span></span>       | <span data-ttu-id="8fd1a-119">说明</span><span class="sxs-lookup"><span data-stu-id="8fd1a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8fd1a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fd1a-120">Authorization</span></span>  | <span data-ttu-id="8fd1a-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8fd1a-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fd1a-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="8fd1a-122">Request body</span></span>
<span data-ttu-id="8fd1a-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8fd1a-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8fd1a-124">响应</span><span class="sxs-lookup"><span data-stu-id="8fd1a-124">Response</span></span>
<span data-ttu-id="8fd1a-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8fd1a-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fd1a-127">示例</span><span class="sxs-lookup"><span data-stu-id="8fd1a-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8fd1a-128">请求</span><span class="sxs-lookup"><span data-stu-id="8fd1a-128">Request</span></span>
<span data-ttu-id="8fd1a-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8fd1a-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="8fd1a-130">响应</span><span class="sxs-lookup"><span data-stu-id="8fd1a-130">Response</span></span>
<span data-ttu-id="8fd1a-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8fd1a-131">The following is an example of the response.</span></span>
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
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
