---
title: 添加 accessReview 审阅者
description: '在 Azure AD 访问评审功能中，更新现有 accessReview 对象以将其他用户添加为审阅者。  仅允许对尚未完成的访问评审进行此操作，并且仅允许对明确指定审阅者的访问评审执行此操作。 不允许此操作进行访问评审，用户在此审阅自己的访问权限时，不应进行组所有者分配为审阅者的访问评审。 '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 90c64ee1bb52c9149e16658c5b8a1cd11a97c51b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751123"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="420b0-105">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="420b0-105">Add accessReview reviewer</span></span>

<span data-ttu-id="420b0-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="420b0-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="420b0-107">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，更新现有 [accessReview](../resources/accessreview.md) 对象以将其他用户添加为审阅者。</span><span class="sxs-lookup"><span data-stu-id="420b0-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="420b0-108">仅允许对尚未完成的访问评审进行此操作，并且仅允许对明确指定审阅者的访问评审执行此操作。</span><span class="sxs-lookup"><span data-stu-id="420b0-108">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="420b0-109">不允许此操作进行访问评审，用户在此审阅自己的访问权限时，不应进行组所有者分配为审阅者的访问评审。</span><span class="sxs-lookup"><span data-stu-id="420b0-109">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="420b0-110">权限</span><span class="sxs-lookup"><span data-stu-id="420b0-110">Permissions</span></span>
<span data-ttu-id="420b0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="420b0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="420b0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="420b0-113">Permission type</span></span>                        | <span data-ttu-id="420b0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="420b0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="420b0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="420b0-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="420b0-116">AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="420b0-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="420b0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="420b0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="420b0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="420b0-118">Not supported.</span></span> |
|<span data-ttu-id="420b0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="420b0-119">Application</span></span>                            | <span data-ttu-id="420b0-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="420b0-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="420b0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="420b0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="420b0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="420b0-122">Request headers</span></span>
| <span data-ttu-id="420b0-123">名称</span><span class="sxs-lookup"><span data-stu-id="420b0-123">Name</span></span>         | <span data-ttu-id="420b0-124">类型</span><span class="sxs-lookup"><span data-stu-id="420b0-124">Type</span></span>        | <span data-ttu-id="420b0-125">说明</span><span class="sxs-lookup"><span data-stu-id="420b0-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="420b0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="420b0-126">Authorization</span></span> | <span data-ttu-id="420b0-127">string</span><span class="sxs-lookup"><span data-stu-id="420b0-127">string</span></span> | <span data-ttu-id="420b0-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="420b0-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="420b0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="420b0-130">Request body</span></span>
<span data-ttu-id="420b0-131">在请求正文中，提供将成为审阅者的用户 ID 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="420b0-131">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="420b0-132">下表显示更新 accessReview 时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="420b0-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="420b0-133">属性</span><span class="sxs-lookup"><span data-stu-id="420b0-133">Property</span></span>     | <span data-ttu-id="420b0-134">类型</span><span class="sxs-lookup"><span data-stu-id="420b0-134">Type</span></span>        | <span data-ttu-id="420b0-135">说明</span><span class="sxs-lookup"><span data-stu-id="420b0-135">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="420b0-136">id</span><span class="sxs-lookup"><span data-stu-id="420b0-136">id</span></span>        | <span data-ttu-id="420b0-137">String</span><span class="sxs-lookup"><span data-stu-id="420b0-137">String</span></span>   | <span data-ttu-id="420b0-138">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="420b0-138">The user ID.</span></span>|


## <a name="response"></a><span data-ttu-id="420b0-139">响应</span><span class="sxs-lookup"><span data-stu-id="420b0-139">Response</span></span>
<span data-ttu-id="420b0-140">如果成功，此方法返回 响应 `201 Created` 代码 。</span><span class="sxs-lookup"><span data-stu-id="420b0-140">If successful, this method returns a `201 Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="420b0-141">示例</span><span class="sxs-lookup"><span data-stu-id="420b0-141">Example</span></span>

<span data-ttu-id="420b0-142">这是一个更新一次检查， (审阅者) 访问评审的示例。</span><span class="sxs-lookup"><span data-stu-id="420b0-142">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="420b0-143">请求</span><span class="sxs-lookup"><span data-stu-id="420b0-143">Request</span></span>
<span data-ttu-id="420b0-144">在请求正文中，提供用户对象的 ID 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="420b0-144">In the request body, supply a JSON representation of the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="420b0-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="420b0-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="420b0-146">C#</span><span class="sxs-lookup"><span data-stu-id="420b0-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="420b0-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="420b0-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="420b0-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="420b0-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="420b0-149">Java</span><span class="sxs-lookup"><span data-stu-id="420b0-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="420b0-150">响应</span><span class="sxs-lookup"><span data-stu-id="420b0-150">Response</span></span>
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


