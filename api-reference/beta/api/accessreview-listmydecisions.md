---
title: 列出我的 accessReview 决策
description: 在 Azure AD 访问评审功能中，检索作为审阅者的调用用户的 accessReview 对象的决策。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a4ab7557b3425987b838335e43219fee802ef513
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751102"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="1c92a-103">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1c92a-103">List my accessReview decisions</span></span>

<span data-ttu-id="1c92a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c92a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c92a-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，检索作为审阅者的调用用户的 [accessReview](../resources/accessreview.md) 对象的决策。</span><span class="sxs-lookup"><span data-stu-id="1c92a-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c92a-106">权限</span><span class="sxs-lookup"><span data-stu-id="1c92a-106">Permissions</span></span>
<span data-ttu-id="1c92a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c92a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c92a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c92a-109">Permission type</span></span>                        | <span data-ttu-id="1c92a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c92a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c92a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c92a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c92a-112">AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c92a-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="1c92a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c92a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c92a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c92a-114">Not supported.</span></span> |
|<span data-ttu-id="1c92a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c92a-115">Application</span></span>                            | <span data-ttu-id="1c92a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c92a-116">Not supported.</span></span> |

<span data-ttu-id="1c92a-117">还必须允许登录用户阅读此特定访问评审。</span><span class="sxs-lookup"><span data-stu-id="1c92a-117">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="1c92a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c92a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="1c92a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c92a-119">Request headers</span></span>
| <span data-ttu-id="1c92a-120">名称</span><span class="sxs-lookup"><span data-stu-id="1c92a-120">Name</span></span>         | <span data-ttu-id="1c92a-121">类型</span><span class="sxs-lookup"><span data-stu-id="1c92a-121">Type</span></span>        | <span data-ttu-id="1c92a-122">说明</span><span class="sxs-lookup"><span data-stu-id="1c92a-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1c92a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c92a-123">Authorization</span></span> | <span data-ttu-id="1c92a-124">string</span><span class="sxs-lookup"><span data-stu-id="1c92a-124">string</span></span> | <span data-ttu-id="1c92a-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c92a-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c92a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c92a-127">Request body</span></span>
<span data-ttu-id="1c92a-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="1c92a-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="1c92a-129">响应</span><span class="sxs-lookup"><span data-stu-id="1c92a-129">Response</span></span>
<span data-ttu-id="1c92a-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewDecision](../resources/accessreviewdecision.md) 对象数组，调用用户为其分配了审阅者。</span><span class="sxs-lookup"><span data-stu-id="1c92a-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="1c92a-131">示例</span><span class="sxs-lookup"><span data-stu-id="1c92a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c92a-132">请求</span><span class="sxs-lookup"><span data-stu-id="1c92a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1c92a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c92a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```
# <a name="c"></a>[<span data-ttu-id="1c92a-134">C#</span><span class="sxs-lookup"><span data-stu-id="1c92a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c92a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c92a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c92a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c92a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c92a-137">Java</span><span class="sxs-lookup"><span data-stu-id="1c92a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1c92a-138">响应</span><span class="sxs-lookup"><span data-stu-id="1c92a-138">Response</span></span>
><span data-ttu-id="1c92a-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1c92a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="1c92a-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1c92a-140">See also</span></span>

| <span data-ttu-id="1c92a-141">方法</span><span class="sxs-lookup"><span data-stu-id="1c92a-141">Method</span></span>           | <span data-ttu-id="1c92a-142">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c92a-142">Return Type</span></span>    |<span data-ttu-id="1c92a-143">Description</span><span class="sxs-lookup"><span data-stu-id="1c92a-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1c92a-144">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="1c92a-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="1c92a-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="1c92a-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="1c92a-146">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="1c92a-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="1c92a-147">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1c92a-147">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="1c92a-148">[accessReviewDecision](../resources/accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c92a-148">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="1c92a-149">检索 accessReview 的所有决策。</span><span class="sxs-lookup"><span data-stu-id="1c92a-149">Retrieve all the decisions of an accessReview.</span></span>|


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


