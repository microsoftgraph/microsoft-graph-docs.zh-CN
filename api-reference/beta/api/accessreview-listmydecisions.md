---
title: 列出我的 accessReview 决策
description: 在 Azure AD 访问评审功能中，检索作为审阅者的调用用户的 accessReview 对象的决策。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 31f065033d1980c8a1ab640294f52f893a1f02f0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048468"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="ef25e-103">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="ef25e-103">List my accessReview decisions</span></span>

<span data-ttu-id="ef25e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef25e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef25e-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，检索作为审阅者的调用用户的 [accessReview](../resources/accessreview.md) 对象的决策。</span><span class="sxs-lookup"><span data-stu-id="ef25e-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef25e-106">权限</span><span class="sxs-lookup"><span data-stu-id="ef25e-106">Permissions</span></span>
<span data-ttu-id="ef25e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef25e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef25e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef25e-109">Permission type</span></span>                        | <span data-ttu-id="ef25e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef25e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef25e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef25e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef25e-112">AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef25e-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="ef25e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef25e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef25e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef25e-114">Not supported.</span></span> |
|<span data-ttu-id="ef25e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef25e-115">Application</span></span>                            | <span data-ttu-id="ef25e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef25e-116">Not supported.</span></span> |

<span data-ttu-id="ef25e-117">还必须允许登录用户阅读此特定访问评审。</span><span class="sxs-lookup"><span data-stu-id="ef25e-117">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="ef25e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef25e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="ef25e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef25e-119">Request headers</span></span>
| <span data-ttu-id="ef25e-120">名称</span><span class="sxs-lookup"><span data-stu-id="ef25e-120">Name</span></span>         | <span data-ttu-id="ef25e-121">类型</span><span class="sxs-lookup"><span data-stu-id="ef25e-121">Type</span></span>        | <span data-ttu-id="ef25e-122">说明</span><span class="sxs-lookup"><span data-stu-id="ef25e-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ef25e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef25e-123">Authorization</span></span> | <span data-ttu-id="ef25e-124">string</span><span class="sxs-lookup"><span data-stu-id="ef25e-124">string</span></span> | <span data-ttu-id="ef25e-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="ef25e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef25e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef25e-127">Request body</span></span>
<span data-ttu-id="ef25e-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="ef25e-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="ef25e-129">响应</span><span class="sxs-lookup"><span data-stu-id="ef25e-129">Response</span></span>
<span data-ttu-id="ef25e-130">如果成功，此方法在响应正文中返回 响应代码和 `200, OK` [accessReviewDecision](../resources/accessreviewdecision.md) 对象数组，调用用户为其分配了审阅者。</span><span class="sxs-lookup"><span data-stu-id="ef25e-130">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="ef25e-131">示例</span><span class="sxs-lookup"><span data-stu-id="ef25e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef25e-132">请求</span><span class="sxs-lookup"><span data-stu-id="ef25e-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ef25e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef25e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```
# <a name="c"></a>[<span data-ttu-id="ef25e-134">C#</span><span class="sxs-lookup"><span data-stu-id="ef25e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef25e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef25e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef25e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef25e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef25e-137">Java</span><span class="sxs-lookup"><span data-stu-id="ef25e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ef25e-138">响应</span><span class="sxs-lookup"><span data-stu-id="ef25e-138">Response</span></span>
><span data-ttu-id="ef25e-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ef25e-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ef25e-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ef25e-140">See also</span></span>

| <span data-ttu-id="ef25e-141">方法</span><span class="sxs-lookup"><span data-stu-id="ef25e-141">Method</span></span>           | <span data-ttu-id="ef25e-142">返回类型</span><span class="sxs-lookup"><span data-stu-id="ef25e-142">Return Type</span></span>    |<span data-ttu-id="ef25e-143">说明</span><span class="sxs-lookup"><span data-stu-id="ef25e-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef25e-144">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="ef25e-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="ef25e-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="ef25e-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="ef25e-146">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="ef25e-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="ef25e-147">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="ef25e-147">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="ef25e-148">[accessReviewDecision](../resources/accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ef25e-148">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="ef25e-149">检索 accessReview 的所有决策。</span><span class="sxs-lookup"><span data-stu-id="ef25e-149">Retrieve all the decisions of an accessReview.</span></span>|


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


