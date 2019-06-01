---
title: 删除 accessReview 审阅者
description: '在 "Azure AD access 评论" 功能中, 更新现有 accessReview 对象以将用户删除为审阅者。  仅允许对尚未完成的访问权限审核执行此操作, 并且仅适用于显式指定审阅者的访问审核。 此操作不允许用于用户查看其自己的访问权限的访问审核, 而不适用于将组所有者分配为审阅者的访问审核。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c0b5407b07f309a1c6e7e5e8e6bd0942ad8aca23
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655535"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="4021b-105">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="4021b-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4021b-106">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 更新现有[accessReview](../resources/accessreview.md)对象以将用户删除为审阅者。</span><span class="sxs-lookup"><span data-stu-id="4021b-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="4021b-107">仅允许对尚未完成的访问权限审核执行此操作, 并且仅适用于显式指定审阅者的访问审核。</span><span class="sxs-lookup"><span data-stu-id="4021b-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="4021b-108">此操作不允许用于用户查看其自己的访问权限的访问审核, 而不适用于将组所有者分配为审阅者的访问审核。</span><span class="sxs-lookup"><span data-stu-id="4021b-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="4021b-109">权限</span><span class="sxs-lookup"><span data-stu-id="4021b-109">Permissions</span></span>
<span data-ttu-id="4021b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4021b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4021b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4021b-112">Permission type</span></span>                        | <span data-ttu-id="4021b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4021b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4021b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4021b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4021b-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4021b-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="4021b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4021b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4021b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4021b-117">Not supported.</span></span> |
|<span data-ttu-id="4021b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4021b-118">Application</span></span>                            | <span data-ttu-id="4021b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="4021b-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4021b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4021b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="4021b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4021b-121">Request headers</span></span>
| <span data-ttu-id="4021b-122">名称</span><span class="sxs-lookup"><span data-stu-id="4021b-122">Name</span></span>         | <span data-ttu-id="4021b-123">类型</span><span class="sxs-lookup"><span data-stu-id="4021b-123">Type</span></span>        | <span data-ttu-id="4021b-124">说明</span><span class="sxs-lookup"><span data-stu-id="4021b-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4021b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4021b-125">Authorization</span></span> | <span data-ttu-id="4021b-126">string</span><span class="sxs-lookup"><span data-stu-id="4021b-126">string</span></span> | <span data-ttu-id="4021b-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="4021b-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4021b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4021b-129">Request body</span></span>
<span data-ttu-id="4021b-130">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="4021b-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="4021b-131">响应</span><span class="sxs-lookup"><span data-stu-id="4021b-131">Response</span></span>
<span data-ttu-id="4021b-132">如果成功, 此方法将返回一个200系列响应代码。</span><span class="sxs-lookup"><span data-stu-id="4021b-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="4021b-133">示例</span><span class="sxs-lookup"><span data-stu-id="4021b-133">Example</span></span>

<span data-ttu-id="4021b-134">这是更新一次性 (不定期) 访问评审以删除不必要的审阅者的示例。</span><span class="sxs-lookup"><span data-stu-id="4021b-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="4021b-135">请求</span><span class="sxs-lookup"><span data-stu-id="4021b-135">Request</span></span>
<span data-ttu-id="4021b-136">在请求 URL 中, 提供 accessReview 对象的 id, 然后提供 user 对象的 id。</span><span class="sxs-lookup"><span data-stu-id="4021b-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```

##### <a name="response"></a><span data-ttu-id="4021b-137">响应</span><span class="sxs-lookup"><span data-stu-id="4021b-137">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4021b-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4021b-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4021b-139">C#</span><span class="sxs-lookup"><span data-stu-id="4021b-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_accessReview_reviewer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4021b-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="4021b-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_accessReview_reviewer-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-removereviewer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-removereviewer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
