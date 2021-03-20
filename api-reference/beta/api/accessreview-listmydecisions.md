---
title: 列出我的 accessReview 决策
description: 在 Azure AD 访问评审功能中，检索作为审阅者的调用用户的 accessReview 对象的决策。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9179a92c103e7645d6b7fc8aa1728b233ca62a5a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943129"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="3c1b4-103">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="3c1b4-103">List my accessReview decisions</span></span>

<span data-ttu-id="3c1b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c1b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c1b4-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，检索作为审阅者的调用用户的 [accessReview](../resources/accessreview.md) 对象的决策。</span><span class="sxs-lookup"><span data-stu-id="3c1b4-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c1b4-106">权限</span><span class="sxs-lookup"><span data-stu-id="3c1b4-106">Permissions</span></span>
<span data-ttu-id="3c1b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c1b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c1b4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c1b4-109">Permission type</span></span>                        | <span data-ttu-id="3c1b4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c1b4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c1b4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c1b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c1b4-112">AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c1b4-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="3c1b4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c1b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c1b4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c1b4-114">Not supported.</span></span> |
|<span data-ttu-id="3c1b4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c1b4-115">Application</span></span>                            | <span data-ttu-id="3c1b4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c1b4-116">Not supported.</span></span> |

<span data-ttu-id="3c1b4-117">还必须允许登录用户阅读此特定访问评审。</span><span class="sxs-lookup"><span data-stu-id="3c1b4-117">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="3c1b4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c1b4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="3c1b4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c1b4-119">Request headers</span></span>
| <span data-ttu-id="3c1b4-120">名称</span><span class="sxs-lookup"><span data-stu-id="3c1b4-120">Name</span></span>         | <span data-ttu-id="3c1b4-121">类型</span><span class="sxs-lookup"><span data-stu-id="3c1b4-121">Type</span></span>        | <span data-ttu-id="3c1b4-122">说明</span><span class="sxs-lookup"><span data-stu-id="3c1b4-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3c1b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c1b4-123">Authorization</span></span> | <span data-ttu-id="3c1b4-124">string</span><span class="sxs-lookup"><span data-stu-id="3c1b4-124">string</span></span> | <span data-ttu-id="3c1b4-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c1b4-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c1b4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c1b4-127">Request body</span></span>
<span data-ttu-id="3c1b4-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c1b4-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="3c1b4-129">响应</span><span class="sxs-lookup"><span data-stu-id="3c1b4-129">Response</span></span>
<span data-ttu-id="3c1b4-130">如果成功，此方法在响应正文中返回 响应代码和 `200, OK` [accessReviewDecision](../resources/accessreviewdecision.md) 对象数组，调用用户为其分配了审阅者。</span><span class="sxs-lookup"><span data-stu-id="3c1b4-130">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="3c1b4-131">示例</span><span class="sxs-lookup"><span data-stu-id="3c1b4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c1b4-132">请求</span><span class="sxs-lookup"><span data-stu-id="3c1b4-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3c1b4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c1b4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```
# <a name="c"></a>[<span data-ttu-id="3c1b4-134">C#</span><span class="sxs-lookup"><span data-stu-id="3c1b4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c1b4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c1b4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c1b4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c1b4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c1b4-137">Java</span><span class="sxs-lookup"><span data-stu-id="3c1b4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3c1b4-138">响应</span><span class="sxs-lookup"><span data-stu-id="3c1b4-138">Response</span></span>
><span data-ttu-id="3c1b4-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3c1b4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3c1b4-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3c1b4-141">See also</span></span>

| <span data-ttu-id="3c1b4-142">方法</span><span class="sxs-lookup"><span data-stu-id="3c1b4-142">Method</span></span>           | <span data-ttu-id="3c1b4-143">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c1b4-143">Return Type</span></span>    |<span data-ttu-id="3c1b4-144">说明</span><span class="sxs-lookup"><span data-stu-id="3c1b4-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3c1b4-145">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="3c1b4-145">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="3c1b4-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="3c1b4-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="3c1b4-147">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="3c1b4-147">Retrieve an access review.</span></span> |
|[<span data-ttu-id="3c1b4-148">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="3c1b4-148">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="3c1b4-149">[accessReviewDecision](../resources/accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c1b4-149">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="3c1b4-150">检索 accessReview 的所有决策。</span><span class="sxs-lookup"><span data-stu-id="3c1b4-150">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


