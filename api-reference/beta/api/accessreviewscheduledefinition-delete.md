---
title: 删除 accessReviewScheduleDefinition
description: 删除 accessReviewScheduleDefinition 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d72e5321cf74e66bd34e48b4d6000715f11ea09d
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000756"
---
# <a name="delete-accessreviewscheduledefinition"></a><span data-ttu-id="4e666-103">删除 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="4e666-103">Delete accessReviewScheduleDefinition</span></span>

<span data-ttu-id="4e666-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e666-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e666-105">删除 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4e666-105">Delete an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4e666-106">权限</span><span class="sxs-lookup"><span data-stu-id="4e666-106">Permissions</span></span>
<span data-ttu-id="4e666-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e666-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e666-109">Permission type</span></span>                        | <span data-ttu-id="4e666-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e666-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e666-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e666-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e666-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e666-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="4e666-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e666-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e666-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e666-114">Not supported.</span></span>|
|<span data-ttu-id="4e666-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e666-115">Application</span></span>                            | <span data-ttu-id="4e666-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e666-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e666-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e666-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="4e666-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e666-118">Request headers</span></span>
<span data-ttu-id="4e666-119">无。</span><span class="sxs-lookup"><span data-stu-id="4e666-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="4e666-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e666-120">Request body</span></span>
<span data-ttu-id="4e666-121">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e666-121">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4e666-122">响应</span><span class="sxs-lookup"><span data-stu-id="4e666-122">Response</span></span>
<span data-ttu-id="4e666-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4e666-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4e666-125">示例</span><span class="sxs-lookup"><span data-stu-id="4e666-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="4e666-126">请求</span><span class="sxs-lookup"><span data-stu-id="4e666-126">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/29f2d16e-9ca6-4052-bbfe-802c48981fd8
```

---

### <a name="response"></a><span data-ttu-id="4e666-127">响应</span><span class="sxs-lookup"><span data-stu-id="4e666-127">Response</span></span>
><span data-ttu-id="4e666-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4e666-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
