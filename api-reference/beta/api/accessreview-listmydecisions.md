---
title: 列出我 accessReview 决策
description: 在 Azure AD 访问评论功能中，为审阅者检索呼叫用户的 accessReview 对象的决策。
localization_priority: Normal
ms.openlocfilehash: 27ae3129810b6019ecf47e23f1e4cc48362df6fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819010"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="f8470-103">列出我 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="f8470-103">List my accessReview decisions</span></span>

> <span data-ttu-id="f8470-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f8470-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8470-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f8470-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8470-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，为审阅者检索呼叫用户的[accessReview](../resources/accessreview.md)对象的决策。</span><span class="sxs-lookup"><span data-stu-id="f8470-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8470-107">权限</span><span class="sxs-lookup"><span data-stu-id="f8470-107">Permissions</span></span>
<span data-ttu-id="f8470-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8470-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8470-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8470-110">Permission type</span></span>                        | <span data-ttu-id="f8470-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8470-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8470-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8470-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8470-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="f8470-113"></span></span>  <span data-ttu-id="f8470-114">此外必须允许登录的用户读取此特定访问审查。</span><span class="sxs-lookup"><span data-stu-id="f8470-114">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="f8470-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8470-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8470-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8470-116">Not supported.</span></span> |
|<span data-ttu-id="f8470-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8470-117">Application</span></span>                            | <span data-ttu-id="f8470-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8470-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8470-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8470-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="f8470-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8470-120">Request headers</span></span>
| <span data-ttu-id="f8470-121">名称</span><span class="sxs-lookup"><span data-stu-id="f8470-121">Name</span></span>         | <span data-ttu-id="f8470-122">类型</span><span class="sxs-lookup"><span data-stu-id="f8470-122">Type</span></span>        | <span data-ttu-id="f8470-123">说明</span><span class="sxs-lookup"><span data-stu-id="f8470-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f8470-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8470-124">Authorization</span></span> | <span data-ttu-id="f8470-125">string</span><span class="sxs-lookup"><span data-stu-id="f8470-125">string</span></span> | <span data-ttu-id="f8470-126">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="f8470-126">Bearer \{token\}.</span></span> <span data-ttu-id="f8470-127">必填。</span><span class="sxs-lookup"><span data-stu-id="f8470-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8470-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8470-128">Request body</span></span>
<span data-ttu-id="f8470-129">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8470-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="f8470-130">响应</span><span class="sxs-lookup"><span data-stu-id="f8470-130">Response</span></span>
<span data-ttu-id="f8470-131">如果成功，此方法返回`200, OK`响应代码和在响应正文中，为其呼叫用户是分配给审阅者[accessReviewDecision](../resources/accessreviewdecision.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="f8470-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="f8470-132">示例</span><span class="sxs-lookup"><span data-stu-id="f8470-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8470-133">请求</span><span class="sxs-lookup"><span data-stu-id="f8470-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="f8470-134">响应</span><span class="sxs-lookup"><span data-stu-id="f8470-134">Response</span></span>
><span data-ttu-id="f8470-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f8470-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f8470-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f8470-137">See also</span></span>

| <span data-ttu-id="f8470-138">方法</span><span class="sxs-lookup"><span data-stu-id="f8470-138">Method</span></span>           | <span data-ttu-id="f8470-139">返回类型</span><span class="sxs-lookup"><span data-stu-id="f8470-139">Return Type</span></span>    |<span data-ttu-id="f8470-140">说明</span><span class="sxs-lookup"><span data-stu-id="f8470-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f8470-141">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="f8470-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="f8470-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="f8470-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="f8470-143">检索访问审阅。</span><span class="sxs-lookup"><span data-stu-id="f8470-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="f8470-144">列表 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="f8470-144">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="f8470-145">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="f8470-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="f8470-146">检索所有 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="f8470-146">Retrieve all the decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
