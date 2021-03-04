---
title: 添加 accessReview 审阅者
description: '在 Azure AD 访问评审功能中，更新现有 accessReview 对象以将其他用户添加为审阅者。  仅允许对尚未完成的访问评审执行此操作，并且仅允许对明确指定审阅者的访问评审执行此操作。 不允许此操作用于访问评审，在此审阅中，用户查看自己的访问权限，而不是用于组所有者被分配为审阅者的访问评审。 '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 86ea5525745933e40121a2906cd4a90fdb7f3179
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439448"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="1bc6e-105">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="1bc6e-105">Add accessReview reviewer</span></span>

<span data-ttu-id="1bc6e-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bc6e-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bc6e-107">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，更新现有 [accessReview](../resources/accessreview.md) 对象以将其他用户添加为审阅者。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="1bc6e-108">仅允许对尚未完成的访问评审执行此操作，并且仅允许对明确指定审阅者的访问评审执行此操作。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-108">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="1bc6e-109">不允许此操作进行访问评审，在此审阅中，用户查看自己的访问权限，而不是用于组所有者被分配为审阅者的访问评审。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-109">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="1bc6e-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="1bc6e-110">Permissions</span></span>
<span data-ttu-id="1bc6e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bc6e-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bc6e-113">Permission type</span></span>                        | <span data-ttu-id="1bc6e-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1bc6e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bc6e-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bc6e-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="1bc6e-116">AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bc6e-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="1bc6e-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bc6e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bc6e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-118">Not supported.</span></span> |
|<span data-ttu-id="1bc6e-119">Application</span><span class="sxs-lookup"><span data-stu-id="1bc6e-119">Application</span></span>                            | <span data-ttu-id="1bc6e-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="1bc6e-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bc6e-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bc6e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="1bc6e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bc6e-122">Request headers</span></span>
| <span data-ttu-id="1bc6e-123">名称</span><span class="sxs-lookup"><span data-stu-id="1bc6e-123">Name</span></span>         | <span data-ttu-id="1bc6e-124">类型</span><span class="sxs-lookup"><span data-stu-id="1bc6e-124">Type</span></span>        | <span data-ttu-id="1bc6e-125">说明</span><span class="sxs-lookup"><span data-stu-id="1bc6e-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1bc6e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bc6e-126">Authorization</span></span> | <span data-ttu-id="1bc6e-127">string</span><span class="sxs-lookup"><span data-stu-id="1bc6e-127">string</span></span> | <span data-ttu-id="1bc6e-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bc6e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bc6e-130">Request body</span></span>
<span data-ttu-id="1bc6e-131">在请求正文中，提供将成为审阅者的用户 ID 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-131">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="1bc6e-132">下表显示了在更新 accessReview 时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="1bc6e-133">属性</span><span class="sxs-lookup"><span data-stu-id="1bc6e-133">Property</span></span>     | <span data-ttu-id="1bc6e-134">类型</span><span class="sxs-lookup"><span data-stu-id="1bc6e-134">Type</span></span>        | <span data-ttu-id="1bc6e-135">说明</span><span class="sxs-lookup"><span data-stu-id="1bc6e-135">Description</span></span> |
|:-------------|:------------|:------------|
| `id`        | `String`   | <span data-ttu-id="1bc6e-136">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-136">The user ID.</span></span>|


## <a name="response"></a><span data-ttu-id="1bc6e-137">响应</span><span class="sxs-lookup"><span data-stu-id="1bc6e-137">Response</span></span>
<span data-ttu-id="1bc6e-138">如果成功，此方法将返回 `201, Created` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-138">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="1bc6e-139">示例</span><span class="sxs-lookup"><span data-stu-id="1bc6e-139">Example</span></span>

<span data-ttu-id="1bc6e-140">这是一个更新一次检查示例， (审阅者) 访问评审。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-140">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="1bc6e-141">请求</span><span class="sxs-lookup"><span data-stu-id="1bc6e-141">Request</span></span>
<span data-ttu-id="1bc6e-142">在请求正文中，提供用户对象的 ID 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-142">In the request body, supply a JSON representation of the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="1bc6e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bc6e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
Content-Type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```
# <a name="c"></a>[<span data-ttu-id="1bc6e-144">C#</span><span class="sxs-lookup"><span data-stu-id="1bc6e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bc6e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bc6e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bc6e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bc6e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1bc6e-147">Java</span><span class="sxs-lookup"><span data-stu-id="1bc6e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1bc6e-148">响应</span><span class="sxs-lookup"><span data-stu-id="1bc6e-148">Response</span></span>
><span data-ttu-id="1bc6e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1bc6e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


