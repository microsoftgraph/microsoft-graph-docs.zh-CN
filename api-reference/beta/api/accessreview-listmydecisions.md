---
title: 列出我 accessReview 决策
description: 在 Azure AD 访问评论功能中，为审阅者检索呼叫用户的 accessReview 对象的决策。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e19e3b0581c995f1b0ef52369d3a3e7545696d1c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525323"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="fe9c8-103">列出我 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="fe9c8-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe9c8-104">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，为审阅者检索呼叫用户的[accessReview](../resources/accessreview.md)对象的决策。</span><span class="sxs-lookup"><span data-stu-id="fe9c8-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe9c8-105">权限</span><span class="sxs-lookup"><span data-stu-id="fe9c8-105">Permissions</span></span>
<span data-ttu-id="fe9c8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe9c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe9c8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe9c8-108">Permission type</span></span>                        | <span data-ttu-id="fe9c8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe9c8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe9c8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe9c8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe9c8-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="fe9c8-111"></span></span>  <span data-ttu-id="fe9c8-112">此外必须允许登录的用户读取此特定访问审查。</span><span class="sxs-lookup"><span data-stu-id="fe9c8-112">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="fe9c8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe9c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe9c8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe9c8-114">Not supported.</span></span> |
|<span data-ttu-id="fe9c8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe9c8-115">Application</span></span>                            | <span data-ttu-id="fe9c8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe9c8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe9c8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe9c8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="fe9c8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe9c8-118">Request headers</span></span>
| <span data-ttu-id="fe9c8-119">名称</span><span class="sxs-lookup"><span data-stu-id="fe9c8-119">Name</span></span>         | <span data-ttu-id="fe9c8-120">类型</span><span class="sxs-lookup"><span data-stu-id="fe9c8-120">Type</span></span>        | <span data-ttu-id="fe9c8-121">说明</span><span class="sxs-lookup"><span data-stu-id="fe9c8-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fe9c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe9c8-122">Authorization</span></span> | <span data-ttu-id="fe9c8-123">string</span><span class="sxs-lookup"><span data-stu-id="fe9c8-123">string</span></span> | <span data-ttu-id="fe9c8-124">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="fe9c8-124">Bearer \{token\}.</span></span> <span data-ttu-id="fe9c8-125">必需。</span><span class="sxs-lookup"><span data-stu-id="fe9c8-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe9c8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe9c8-126">Request body</span></span>
<span data-ttu-id="fe9c8-127">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe9c8-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="fe9c8-128">响应</span><span class="sxs-lookup"><span data-stu-id="fe9c8-128">Response</span></span>
<span data-ttu-id="fe9c8-129">如果成功，此方法返回`200, OK`响应代码和在响应正文中，为其呼叫用户是分配给审阅者[accessReviewDecision](../resources/accessreviewdecision.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="fe9c8-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="fe9c8-130">示例</span><span class="sxs-lookup"><span data-stu-id="fe9c8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe9c8-131">请求</span><span class="sxs-lookup"><span data-stu-id="fe9c8-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="fe9c8-132">响应</span><span class="sxs-lookup"><span data-stu-id="fe9c8-132">Response</span></span>
><span data-ttu-id="fe9c8-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fe9c8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="fe9c8-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fe9c8-135">See also</span></span>

| <span data-ttu-id="fe9c8-136">方法</span><span class="sxs-lookup"><span data-stu-id="fe9c8-136">Method</span></span>           | <span data-ttu-id="fe9c8-137">返回类型</span><span class="sxs-lookup"><span data-stu-id="fe9c8-137">Return Type</span></span>    |<span data-ttu-id="fe9c8-138">说明</span><span class="sxs-lookup"><span data-stu-id="fe9c8-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe9c8-139">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="fe9c8-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="fe9c8-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="fe9c8-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="fe9c8-141">检索访问审阅。</span><span class="sxs-lookup"><span data-stu-id="fe9c8-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="fe9c8-142">列表 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="fe9c8-142">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="fe9c8-143">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="fe9c8-143">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="fe9c8-144">检索所有 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="fe9c8-144">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
