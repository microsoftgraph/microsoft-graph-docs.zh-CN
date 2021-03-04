---
title: 列出 accessReview 审阅者
description: 在 Azure AD 访问评审功能中，检索 accessReview 对象的审阅者。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7d77ac50435a9923ec8e504a135e36c6b406f764
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439306"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="6415f-103">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="6415f-103">List accessReview reviewers</span></span>

<span data-ttu-id="6415f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6415f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6415f-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，检索 [accessReview](../resources/accessreview.md) 对象的审阅者。</span><span class="sxs-lookup"><span data-stu-id="6415f-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6415f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6415f-106">Permissions</span></span>
<span data-ttu-id="6415f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6415f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6415f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6415f-109">Permission type</span></span>                        | <span data-ttu-id="6415f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6415f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6415f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6415f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6415f-112">AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6415f-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="6415f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6415f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6415f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6415f-114">Not supported.</span></span> |
|<span data-ttu-id="6415f-115">Application</span><span class="sxs-lookup"><span data-stu-id="6415f-115">Application</span></span>                            | <span data-ttu-id="6415f-116">AccessReview.Read.All、AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="6415f-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |


 <span data-ttu-id="6415f-117">登录用户还必须具有允许其读取访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="6415f-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="6415f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6415f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="6415f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6415f-119">Request headers</span></span>
| <span data-ttu-id="6415f-120">名称</span><span class="sxs-lookup"><span data-stu-id="6415f-120">Name</span></span>         | <span data-ttu-id="6415f-121">类型</span><span class="sxs-lookup"><span data-stu-id="6415f-121">Type</span></span>        | <span data-ttu-id="6415f-122">说明</span><span class="sxs-lookup"><span data-stu-id="6415f-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6415f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6415f-123">Authorization</span></span> | <span data-ttu-id="6415f-124">string</span><span class="sxs-lookup"><span data-stu-id="6415f-124">string</span></span> | <span data-ttu-id="6415f-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="6415f-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6415f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6415f-127">Request body</span></span>
<span data-ttu-id="6415f-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="6415f-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="6415f-129">响应</span><span class="sxs-lookup"><span data-stu-id="6415f-129">Response</span></span>
<span data-ttu-id="6415f-130">如果成功，此方法在响应正文中返回响应代码和 `200, OK` [userIdentity](../resources/useridentity.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="6415f-130">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6415f-131">示例</span><span class="sxs-lookup"><span data-stu-id="6415f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6415f-132">请求</span><span class="sxs-lookup"><span data-stu-id="6415f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6415f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6415f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="c"></a>[<span data-ttu-id="6415f-134">C#</span><span class="sxs-lookup"><span data-stu-id="6415f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6415f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6415f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6415f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6415f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6415f-137">Java</span><span class="sxs-lookup"><span data-stu-id="6415f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-reviewers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6415f-138">响应</span><span class="sxs-lookup"><span data-stu-id="6415f-138">Response</span></span>
><span data-ttu-id="6415f-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6415f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userIdentity",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":
    [
        {
            "id":"006111db-0810-4494-a6df-904d368bd81b"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="6415f-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6415f-141">See also</span></span>

| <span data-ttu-id="6415f-142">方法</span><span class="sxs-lookup"><span data-stu-id="6415f-142">Method</span></span>           | <span data-ttu-id="6415f-143">返回类型</span><span class="sxs-lookup"><span data-stu-id="6415f-143">Return Type</span></span>    |<span data-ttu-id="6415f-144">说明</span><span class="sxs-lookup"><span data-stu-id="6415f-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6415f-145">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="6415f-145">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="6415f-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="6415f-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="6415f-147">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="6415f-147">Retrieve an access review.</span></span> |
|[<span data-ttu-id="6415f-148">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="6415f-148">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="6415f-149">无。</span><span class="sxs-lookup"><span data-stu-id="6415f-149">None.</span></span>   |   <span data-ttu-id="6415f-150">将审阅者添加到 accessReview。</span><span class="sxs-lookup"><span data-stu-id="6415f-150">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="6415f-151">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="6415f-151">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="6415f-152">无。</span><span class="sxs-lookup"><span data-stu-id="6415f-152">None.</span></span> |   <span data-ttu-id="6415f-153">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="6415f-153">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


