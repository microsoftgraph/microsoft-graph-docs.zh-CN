---
title: 添加 accessReview 审阅者
description: '在 "Azure AD access 评论" 功能中, 更新现有的 accessReview 对象以将其他用户添加为审阅者。  仅允许对尚未完成的访问权限审核执行此操作, 并且仅适用于显式指定审阅者的访问审核。 此操作不允许用于用户查看其自己的访问权限的访问审核, 而不适用于将组所有者分配为审阅者的访问审核。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: aa07b58401aab8dd20f768cbee77bbe55d8eb27a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586315"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="dfcd5-105">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="dfcd5-105">Add accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfcd5-106">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 更新现有的[accessReview](../resources/accessreview.md)对象以将其他用户添加为审阅者。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="dfcd5-107">仅允许对尚未完成的访问权限审核执行此操作, 并且仅适用于显式指定审阅者的访问审核。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="dfcd5-108">此操作不允许用于用户查看其自己的访问权限的访问审核, 而不适用于将组所有者分配为审阅者的访问审核。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="dfcd5-109">权限</span><span class="sxs-lookup"><span data-stu-id="dfcd5-109">Permissions</span></span>
<span data-ttu-id="dfcd5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfcd5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfcd5-112">Permission type</span></span>                        | <span data-ttu-id="dfcd5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dfcd5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfcd5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfcd5-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfcd5-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfcd5-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="dfcd5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfcd5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfcd5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-117">Not supported.</span></span> |
|<span data-ttu-id="dfcd5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfcd5-118">Application</span></span>                            | <span data-ttu-id="dfcd5-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfcd5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfcd5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="dfcd5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfcd5-121">Request headers</span></span>
| <span data-ttu-id="dfcd5-122">名称</span><span class="sxs-lookup"><span data-stu-id="dfcd5-122">Name</span></span>         | <span data-ttu-id="dfcd5-123">类型</span><span class="sxs-lookup"><span data-stu-id="dfcd5-123">Type</span></span>        | <span data-ttu-id="dfcd5-124">说明</span><span class="sxs-lookup"><span data-stu-id="dfcd5-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="dfcd5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfcd5-125">Authorization</span></span> | <span data-ttu-id="dfcd5-126">string</span><span class="sxs-lookup"><span data-stu-id="dfcd5-126">string</span></span> | <span data-ttu-id="dfcd5-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfcd5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfcd5-129">Request body</span></span>
<span data-ttu-id="dfcd5-130">在请求正文中, 提供将成为审阅者的用户 ID 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-130">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="dfcd5-131">下表显示了在更新 accessReview 时可提供的属性。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="dfcd5-132">属性</span><span class="sxs-lookup"><span data-stu-id="dfcd5-132">Property</span></span>     | <span data-ttu-id="dfcd5-133">类型</span><span class="sxs-lookup"><span data-stu-id="dfcd5-133">Type</span></span>        | <span data-ttu-id="dfcd5-134">说明</span><span class="sxs-lookup"><span data-stu-id="dfcd5-134">Description</span></span> |
|:-------------|:------------|:------------|
| `id`        | `String`   | <span data-ttu-id="dfcd5-135">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-135">The user ID.</span></span>|


## <a name="response"></a><span data-ttu-id="dfcd5-136">响应</span><span class="sxs-lookup"><span data-stu-id="dfcd5-136">Response</span></span>
<span data-ttu-id="dfcd5-137">如果成功, 此方法将`201, Created`返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-137">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="dfcd5-138">示例</span><span class="sxs-lookup"><span data-stu-id="dfcd5-138">Example</span></span>

<span data-ttu-id="dfcd5-139">以下是使用其他审阅者更新一次性 (不定期) 访问评审的示例。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-139">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="dfcd5-140">请求</span><span class="sxs-lookup"><span data-stu-id="dfcd5-140">Request</span></span>
<span data-ttu-id="dfcd5-141">在请求正文中, 提供 user 对象的 id 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-141">In the request body, supply a JSON representation of the id of the user object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="dfcd5-142">响应</span><span class="sxs-lookup"><span data-stu-id="dfcd5-142">Response</span></span>
><span data-ttu-id="dfcd5-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dfcd5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfcd5-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dfcd5-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfcd5-146">语言</span><span class="sxs-lookup"><span data-stu-id="dfcd5-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/add_accessReview_reviewer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfcd5-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfcd5-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/add_accessReview_reviewer-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-addreviewer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-addreviewer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
