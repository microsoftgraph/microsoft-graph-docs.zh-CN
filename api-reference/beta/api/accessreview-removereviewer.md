---
title: 删除 accessReview 审阅者
description: 删除 access 审阅审阅者。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 88a4fdcb6b50377c232c051e287681b0e41828ef
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123529"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="c6368-103">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="c6368-103">Remove accessReview reviewer</span></span>

<span data-ttu-id="c6368-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6368-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6368-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中，更新现有[accessReview](../resources/accessreview.md)对象以将用户删除为审阅者。</span><span class="sxs-lookup"><span data-stu-id="c6368-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="c6368-106">仅允许对尚未完成的访问权限审核执行此操作，并且仅适用于显式指定审阅者的访问审核。</span><span class="sxs-lookup"><span data-stu-id="c6368-106">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="c6368-107">此操作不允许用于用户查看其自己的访问权限的访问审核，而不适用于将组所有者分配为审阅者的访问审核。</span><span class="sxs-lookup"><span data-stu-id="c6368-107">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="c6368-108">权限</span><span class="sxs-lookup"><span data-stu-id="c6368-108">Permissions</span></span>
<span data-ttu-id="c6368-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6368-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6368-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6368-111">Permission type</span></span>                        | <span data-ttu-id="c6368-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6368-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6368-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6368-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6368-114">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="c6368-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="c6368-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6368-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6368-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6368-116">Not supported.</span></span> |
|<span data-ttu-id="c6368-117">Application</span><span class="sxs-lookup"><span data-stu-id="c6368-117">Application</span></span>                            | <span data-ttu-id="c6368-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="c6368-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6368-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6368-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}/reviewers/{userId}
```
## <a name="request-headers"></a><span data-ttu-id="c6368-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6368-120">Request headers</span></span>
| <span data-ttu-id="c6368-121">名称</span><span class="sxs-lookup"><span data-stu-id="c6368-121">Name</span></span>         | <span data-ttu-id="c6368-122">类型</span><span class="sxs-lookup"><span data-stu-id="c6368-122">Type</span></span>        | <span data-ttu-id="c6368-123">说明</span><span class="sxs-lookup"><span data-stu-id="c6368-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c6368-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6368-124">Authorization</span></span> | <span data-ttu-id="c6368-125">string</span><span class="sxs-lookup"><span data-stu-id="c6368-125">string</span></span> | <span data-ttu-id="c6368-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6368-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6368-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6368-128">Request body</span></span>
<span data-ttu-id="c6368-129">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="c6368-129">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="c6368-130">响应</span><span class="sxs-lookup"><span data-stu-id="c6368-130">Response</span></span>
<span data-ttu-id="c6368-131">如果成功，此方法将返回一个200系列响应代码。</span><span class="sxs-lookup"><span data-stu-id="c6368-131">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="c6368-132">示例</span><span class="sxs-lookup"><span data-stu-id="c6368-132">Example</span></span>

<span data-ttu-id="c6368-133">这是更新一次性（不定期）访问评审以删除不必要的审阅者的示例。</span><span class="sxs-lookup"><span data-stu-id="c6368-133">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="c6368-134">请求</span><span class="sxs-lookup"><span data-stu-id="c6368-134">Request</span></span>
<span data-ttu-id="c6368-135">在请求 URL 中，提供 accessReview 对象的 id，然后提供 user 对象的 id。</span><span class="sxs-lookup"><span data-stu-id="c6368-135">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="c6368-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6368-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="c"></a>[<span data-ttu-id="c6368-137">C#</span><span class="sxs-lookup"><span data-stu-id="c6368-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6368-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6368-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6368-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6368-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c6368-140">响应</span><span class="sxs-lookup"><span data-stu-id="c6368-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
