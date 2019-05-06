---
title: 列出 accessReview 审阅者
description: 在 "Azure AD access 评论" 功能中, 检索 accessReview 对象的审阅者。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 756cb2d7bc93ea8fe490d0f857c609c3f82229f6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33585988"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="dfd75-103">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="dfd75-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfd75-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 检索[accessReview](../resources/accessreview.md)对象的审阅者。</span><span class="sxs-lookup"><span data-stu-id="dfd75-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dfd75-105">权限</span><span class="sxs-lookup"><span data-stu-id="dfd75-105">Permissions</span></span>
<span data-ttu-id="dfd75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfd75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfd75-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfd75-108">Permission type</span></span>                        | <span data-ttu-id="dfd75-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dfd75-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfd75-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfd75-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfd75-111">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="dfd75-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="dfd75-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfd75-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfd75-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfd75-113">Not supported.</span></span> |
|<span data-ttu-id="dfd75-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfd75-114">Application</span></span>                            | <span data-ttu-id="dfd75-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfd75-115">AccessReview.Read.All</span></span>  |


 <span data-ttu-id="dfd75-116">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="dfd75-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="dfd75-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfd75-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="dfd75-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfd75-118">Request headers</span></span>
| <span data-ttu-id="dfd75-119">名称</span><span class="sxs-lookup"><span data-stu-id="dfd75-119">Name</span></span>         | <span data-ttu-id="dfd75-120">类型</span><span class="sxs-lookup"><span data-stu-id="dfd75-120">Type</span></span>        | <span data-ttu-id="dfd75-121">说明</span><span class="sxs-lookup"><span data-stu-id="dfd75-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="dfd75-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfd75-122">Authorization</span></span> | <span data-ttu-id="dfd75-123">string</span><span class="sxs-lookup"><span data-stu-id="dfd75-123">string</span></span> | <span data-ttu-id="dfd75-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="dfd75-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfd75-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfd75-126">Request body</span></span>
<span data-ttu-id="dfd75-127">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="dfd75-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="dfd75-128">响应</span><span class="sxs-lookup"><span data-stu-id="dfd75-128">Response</span></span>
<span data-ttu-id="dfd75-129">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[userIdentity](../resources/useridentity.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="dfd75-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfd75-130">示例</span><span class="sxs-lookup"><span data-stu-id="dfd75-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfd75-131">请求</span><span class="sxs-lookup"><span data-stu-id="dfd75-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```

##### <a name="response"></a><span data-ttu-id="dfd75-132">响应</span><span class="sxs-lookup"><span data-stu-id="dfd75-132">Response</span></span>
><span data-ttu-id="dfd75-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dfd75-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfd75-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dfd75-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfd75-136">语言</span><span class="sxs-lookup"><span data-stu-id="dfd75-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_reviewers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfd75-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfd75-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_reviewers-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="dfd75-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="dfd75-138">See also</span></span>

| <span data-ttu-id="dfd75-139">方法</span><span class="sxs-lookup"><span data-stu-id="dfd75-139">Method</span></span>           | <span data-ttu-id="dfd75-140">返回类型</span><span class="sxs-lookup"><span data-stu-id="dfd75-140">Return Type</span></span>    |<span data-ttu-id="dfd75-141">说明</span><span class="sxs-lookup"><span data-stu-id="dfd75-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dfd75-142">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="dfd75-142">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="dfd75-143">accessReview</span><span class="sxs-lookup"><span data-stu-id="dfd75-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="dfd75-144">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="dfd75-144">Retrieve an access review.</span></span> |
|[<span data-ttu-id="dfd75-145">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="dfd75-145">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="dfd75-146">无。</span><span class="sxs-lookup"><span data-stu-id="dfd75-146">None.</span></span>   |   <span data-ttu-id="dfd75-147">向 accessReview 添加审阅者。</span><span class="sxs-lookup"><span data-stu-id="dfd75-147">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="dfd75-148">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="dfd75-148">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="dfd75-149">无。</span><span class="sxs-lookup"><span data-stu-id="dfd75-149">None.</span></span> |   <span data-ttu-id="dfd75-150">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="dfd75-150">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
