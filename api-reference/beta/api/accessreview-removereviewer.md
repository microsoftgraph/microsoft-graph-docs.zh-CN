---
title: 删除 accessReview 审阅者
description: 删除访问评审审阅者。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 83f136a3a9c131d5a05df92df2f3c3e3d3b6c75c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439297"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="311d2-103">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="311d2-103">Remove accessReview reviewer</span></span>

<span data-ttu-id="311d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="311d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="311d2-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，更新现有 [accessReview](../resources/accessreview.md) 对象以删除作为审阅者的用户。</span><span class="sxs-lookup"><span data-stu-id="311d2-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="311d2-106">仅允许对尚未完成的访问评审执行此操作，并且仅允许对明确指定审阅者的访问评审执行此操作。</span><span class="sxs-lookup"><span data-stu-id="311d2-106">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="311d2-107">不允许此操作进行访问评审，在此审阅中，用户查看自己的访问权限，而不是用于组所有者被分配为审阅者的访问评审。</span><span class="sxs-lookup"><span data-stu-id="311d2-107">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="311d2-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="311d2-108">Permissions</span></span>
<span data-ttu-id="311d2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="311d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="311d2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="311d2-111">Permission type</span></span>                        | <span data-ttu-id="311d2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="311d2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="311d2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="311d2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="311d2-114">AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="311d2-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="311d2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="311d2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="311d2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="311d2-116">Not supported.</span></span> |
|<span data-ttu-id="311d2-117">Application</span><span class="sxs-lookup"><span data-stu-id="311d2-117">Application</span></span>                            | <span data-ttu-id="311d2-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="311d2-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="311d2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="311d2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}/reviewers/{userId}
```
## <a name="request-headers"></a><span data-ttu-id="311d2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="311d2-120">Request headers</span></span>
| <span data-ttu-id="311d2-121">名称</span><span class="sxs-lookup"><span data-stu-id="311d2-121">Name</span></span>         | <span data-ttu-id="311d2-122">类型</span><span class="sxs-lookup"><span data-stu-id="311d2-122">Type</span></span>        | <span data-ttu-id="311d2-123">说明</span><span class="sxs-lookup"><span data-stu-id="311d2-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="311d2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="311d2-124">Authorization</span></span> | <span data-ttu-id="311d2-125">string</span><span class="sxs-lookup"><span data-stu-id="311d2-125">string</span></span> | <span data-ttu-id="311d2-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="311d2-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="311d2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="311d2-128">Request body</span></span>
<span data-ttu-id="311d2-129">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="311d2-129">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="311d2-130">响应</span><span class="sxs-lookup"><span data-stu-id="311d2-130">Response</span></span>
<span data-ttu-id="311d2-131">如果成功，此方法将返回 200 系列响应代码。</span><span class="sxs-lookup"><span data-stu-id="311d2-131">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="311d2-132">示例</span><span class="sxs-lookup"><span data-stu-id="311d2-132">Example</span></span>

<span data-ttu-id="311d2-133">这是一个更新一次检查 (不重复) 访问评审以删除不必要的审阅者的示例。</span><span class="sxs-lookup"><span data-stu-id="311d2-133">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="311d2-134">请求</span><span class="sxs-lookup"><span data-stu-id="311d2-134">Request</span></span>
<span data-ttu-id="311d2-135">在请求 URL 中，提供 accessReview 对象的 ID，然后提供用户对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="311d2-135">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="311d2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="311d2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="c"></a>[<span data-ttu-id="311d2-137">C#</span><span class="sxs-lookup"><span data-stu-id="311d2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="311d2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="311d2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="311d2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="311d2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="311d2-140">Java</span><span class="sxs-lookup"><span data-stu-id="311d2-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="311d2-141">响应</span><span class="sxs-lookup"><span data-stu-id="311d2-141">Response</span></span>
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


